# steenzout-cfg

[![Code Climate](https://codeclimate.com/github/steenzout/steenzout-cfg.png)](https://codeclimate.com/github/steenzout/steenzout-cfg)
[![Gem Version](https://badge.fury.io/rb/steenzout-cfg.svg)](http://badge.fury.io/rb/steenzout-cfg)
[![steenzout-cfg API Documentation](https://www.omniref.com/ruby/gems/steenzout-cfg.png)](https://www.omniref.com/ruby/gems/steenzout-cfg)

steenzout-cfg is a gem to manage configurations.



## convention

On your YAML configuration files, the gem name should be the first element.

<pre><code>gem1:
  (...)
  property: value

gem2:
  (...)
  property: value</pre><code>



## usage

<pre><code>require 'rubygems
require 'steenzout-cfg'

# load the configuration
Steenzout::ConfigurationManager.load 'configuration.yaml'

# access a specific gem configuration
config = Steenzout::ConfigurationManager.configuration_for_gem 'steenzout-cfg'</code></pre>
