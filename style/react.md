# React Style Guide

## Structure Class
    React.createClass({
        
        propTypes: {
            arrayProp: React.PropTypes.array,
            boolProp: React.PropTypes.bool,
            funcProp: React.PropTypes.func,
            numProp: React.PropTypes.number,
            objProp: React.PropTypes.object,
            stringProp: React.PropTypes.string,
        },

        getInitialState: function() {},
        getDefaultProps: function() {},

        componentDidMount : function() {},
        componentDidUpdate : function() {},
        componentWillMount : function() {},
        componentWillReceiveProps: function() {},
        componentWillUnmount : function() {},

        // Custom methods
        parseData : function() {},
        onSelect : function() {},

        // Render method
        render : function() {}

    })