# Postgres Explain Visualizer (pev)

Postgres Explain Visualizer (dev) is designed to make [EXPLAIN](http://www.postgresql.org/docs/current/static/sql-explain.html) output easier to grok. It creates a graphical representation of the plan. You can see it in action at [tatiyants.com/pev](http://tatiyants.com/pev/), or read about it [on my blog](http://tatiyants.com/postgres-query-plan-visualization/).

Pev is heavily influenced by the excellent [explain.depesz.com](http://explain.depesz.com/).

Pev is written in [angular 2](https://angular.io/) with [TypeScript](http://www.typescriptlang.org/). The project is based on [angular2 seed](https://github.com/mgechev/angular2-seed). It requires [npm](https://www.npmjs.com/), [gulp](http://gulpjs.com/), [tsd](http://definitelytyped.org/tsd/), and [compass](http://compass-style.org/).


## Installation

```
npm install
npm start
```

You may also need to install tsd and compass:

```
npm install tsd -g
gem install compass
```

## Build
To build, run the build command for a specific environment. For example, the following will create a production distribution:

```
npm start build.prod
```


```
EXPLAIN (ANALYZE, COSTS, VERBOSE, BUFFERS, FORMAT JSON)
SELECT com_id, com_text
  FROM public.t_comments
  LEFT JOIN t_comments_closure ON com_id = ancestor;
```


http://tatiyants.com/postgres-query-plan-visualization/<br />
https://github.com/AlexTatiyants/pev<br />

https://stackoverflow.com/questions/32624414/text-size-limitation-in-pgadmin-query<br />
http://tatiyants.com/pev/#/plans/new<br />
http://tatiyants.com/pev/#/about<br />

https://explain.depesz.com/<br />
