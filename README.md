# BalancedBinningReference - a package for yellowbrick

## Author: 
Juan L. Kehoe (juanluo2008@gmail.com)

## Purpose:
Implements histogram with vertical lines to help with balanced binning.

## Note:
    BalancedBinningReference allows to generate a histogram with vertical lines
    showing the recommended value point to bin your data so they can be evenly
    distributed in each bin.

    Parameters
    ----------
    ax: matplotlib Axes, default: None
        This is inherited from FeatureVisualizer and is defined within
        BalancedBinningReference.
    feature: string, default: None
        The name of the X variable
        If a DataFrame is passed to fit and feature is None, feature
        is selected as the column of the DataFrame.  There must be only
        one column in the DataFrame.
    target: string, default: None
        The name of the Y variable
        If target is None and a y value is passed to fit then the target
        is selected from the target vector.
    size: float, default: 600
        Size of each side of the figure in pixels
    ratio: float, default: 5
        Ratio of joint axis size to the x and y axes height
    space: float, default: 0.2
        Space between the joint axis and the x and y axes
    kwargs : dict
        Keyword arguments that are passed to the base class and may influence
        the visualization as defined in other Visualizers.

    Examples
    --------
    >>> visualizer = BalancedBinningReference()
    >>> visualizer.fit(X)
    >>> visualizer.poof()


    Notes
    -----
    These parameters can be influenced later on in the visualization
    process, but can and should be set as early as possible.
