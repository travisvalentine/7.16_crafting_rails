!SLIDE center
# [Crafting Rails Applications: Expert Practices for Everyday Rails Development](http://www.amazon.com/Crafting-Rails-Applications-Development-Programmers/dp/1934356735/ref=wl_it_dp_v_S_nC?ie=UTF8&coliid=I9J4XAYHBBMGA&colid=K7D6CDDMZG6S) #

!SLIDE
# The Author - José Valim #

![Jose](tendervalim.jpg)

!SLIDE bullets incremental
# The Disclaimer #

* Everyday is a reach
* Great for those who want to dig into source
* 7 tutorials, each built using TDD with Rails 3.0.3
* Not for beginners

!SLIDE bullets incremental
# Topics covered #

* Templates, Responders, Engines, Railties, Routing, Rack, Instruments, and more.

!SLIDE bullets
# Main Tool: Enginex #

* gem that generates a bare gem
* think `rails new project`

!SLIDE 
# Chapter-by-chapter #

!SLIDE
# This book does things like... #

!SLIDE bullets
# customize `render` #

* `ActionController::Renderers.add :pdf do |filename, options|`

!SLIDE bullets
# create a mail gem #

* Protip: At the end of the chapter, José links to a gem that his company maintains that does what he builds but has more functionality. It's called [Mail Form](https://github.com/plataformatec/mail_form).

!SLIDE bullets
# customize templates #

* Using Resolver API and `virtual_path`
* Resolver API has one method called `find_all`

!SLIDE bullets
# create a new template handler (MERB) #

* Configure new template with railtie `class Railtie < Rails::Railtie`
* `config.generators.mailer :template_engine => :merb`

!SLIDE bullets
# work with Rails engines #

* You can use engines to specify paths
* `class Engine < Rails::Engine`
* `paths.app.controllers = "lib/controllers"`
* `end`

!SLIDE bullets
# work with responders #

!SLIDE bullets
# customize `I18n` #

!SLIDE bullets
# Ever wonder how... #

* `_determine_template` and `_render_template` work
* `to_key` is used by `dom_id` in views
* the `persisted?` method is used in controllers and views
* To create I18n flash messages

!SLIDE bullets
# Or are intrigued by... #

* The fact that each validation is a class (ex: `PresenceValidator`)

!SLIDE bullets
# Or love facts like... #

* Rails, before a request, automatically converts `controller#action` to a Rack application.

!SLIDE
# Then this is a book for you #

!SLIDE bullets
# Key Takeaway #

* `git clone https://github.com/rails/rails.git`
* `cd rails`
* READ SOURCE

!SLIDE
# Thanks #