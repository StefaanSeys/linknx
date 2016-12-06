This repository was cloned from the master branch of the original linknx repository on github on December 5, 2016.

Features added in this version (v0.0.1.34STS):

- Request whether all objects have been initialized:

```
echo -ne '<read><initialized/></read>\x04' | netcat localhost 1030

<read status="success">
        <initialized>
                <value>1</value>
        </initialized>
</read>
```

- Make object deletion easier by allowing automatic stopping and re-enabling of notification listeners:

```
<write><config reset_notifications=1><objects><object id="bla" delete="true"/></objects></config></write>
```

# Documentation
Read the [wiki pages](https://sourceforge.net/p/linknx/wiki/Main_Page/) on sourceforge.

# Downloads
## v0.0.1.33
This is the latest version as of today. You can download a zip
of it [here](https://github.com/linknx/linknx/archive/v0.0.1.33.zip).

## v0.0.1.32
This is the latest version accessible from the legacy repository on sourceforge. You can download a zip
of it [here](https://github.com/linknx/linknx/archive/v0.0.1.32.zip).

