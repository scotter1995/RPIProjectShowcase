<template>
  <div>
    <div v-bind:key="project.id" v-for="project in projects">
      <div v-if="$route.path === '/projects/' + project.title.trim().toLowerCase()">
        <h1>This is the {{project.title}} page</h1>
        <table style="height: 5px;" width="707">
          <tbody>
            <tr>
              <td style="width: 697px;">Here is the name of the project you just clicked on</td>
            </tr>
            <tr>
              <td style="width: 697px;">Credits: Team_member 0, Team_member 1, Team_member 2</td>
            </tr>
            <tr>
              <td style="width: 697px;">Tags: Vue, HTML, small team</td>
            </tr>
          </tbody>
        </table>
        <table style="height: 467px; float: right;" width="276">
          <tbody>
            <tr style="height: 30px;">
              <td style="width: 266px; height: 30px;">
                &nbsp;
                <img
                  src="https://yt3.ggpht.com/a/AATXAJzlav8qcQpxa3wNg8VCah3dskSCiaP5Zrb3kw=s100-c-k-c0xffffffff-no-rj-mo"
                  alt="standard pfp"
                  width="90"
                  height="90"
                />
                <table style="height: 143px; float: right;" width="167">
                  <tbody>
                    <tr>
                      <td style="width: 157px;">Pd.names[0]</td>
                    </tr>
                    <tr>
                      <td style="width: 157px;">pd.majors[0]</td>
                    </tr>
                    <tr>
                      <td style="width: 157px;">pd.projroles[0]</td>
                    </tr>
                    <tr>
                      <td style="width: 157px;">
                        <p>loop and print through pairs of pd.contacts for both icon and contact info</p>
                      </td>
                    </tr>
                  </tbody>
                </table>
              </td>
            </tr>
            <tr style="height: 102px;">
              <td style="width: 266px; height: 102px;">
                &nbsp;
                <img src="https://i.imgur.com/5MM4Uqw.jpg" alt="man" width="100" height="100" />
                <table style="float: right;" width="139">
                  <tbody>
                    <tr>
                      <td>John Snow</td>
                    </tr>
                    <tr>
                      <td>CS</td>
                    </tr>
                    <tr>
                      <td>Project lead</td>
                    </tr>
                    <tr>
                      <td>
                        <img
                          src="https://pbs.twimg.com/profile_images/1212820842712727552/XCuWn8yF_400x400.jpg"
                          alt
                          width="24"
                          height="24"
                        />johndoe#1337
                      </td>
                    </tr>
                  </tbody>
                </table>
              </td>
            </tr>
            <tr style="height: 84px;">
              <td style="width: 266px; height: 84px;">
                &nbsp;
                <img
                  src="https://i.kym-cdn.com/entries/icons/original/000/015/266/Z7HeRxU.png"
                  alt="stock pfp"
                  width="100"
                  height="100"
                />
                <table style="float: right;" width="139">
                  <tbody>
                    <tr>
                      <td>Team_member 2</td>
                    </tr>
                    <tr>
                      <td>CS</td>
                    </tr>
                    <tr>
                      <td>Project lead</td>
                    </tr>
                    <tr>
                      <td>
                        <img
                          src="https://pbs.twimg.com/profile_images/1212820842712727552/XCuWn8yF_400x400.jpg"
                          alt
                          width="24"
                          height="24"
                        />johndoe#1337
                      </td>
                    </tr>
                  </tbody>
                </table>
              </td>
            </tr>
          </tbody>
        </table>
        <p>
          <img
            src="https://logodix.com/logo/2145152.jpg"
            alt="RPI Logo - LogoDix"
            width="401"
            height="399"
          />
        </p>
        <table style="height: 132px;" width="790">
          <tbody>
            <tr>
              <td style="width: 780px;">
                <p>PRoject description</p>
                <p>Lorem ipsum dolor sit amet, consectetur adipiscing elit. Nunc velit risus, tristique vel tortor non, euismod blandit erat. Maecenas ac pharetra dui. Fusce condimentum ex tincidunt, posuere risus at, dictum mi. Vestibulum mollis lorem nec urna egestas, sit amet eleifend dolor auctor. Nullam nec nunc congue quam sollicitudin placerat vel vel elit. Quisque lacinia euismod orci, at rutrum mi ullamcorper vel. Suspendisse metus nibh, volutpat nec ultrices ut, porttitor sed velit.</p>
                <p>Nullam non tellus odio. Nulla consequat, dui vel convallis venenatis, mi ligula laoreet orci, sed convallis nunc leo nec sem. Suspendisse accumsan turpis tristique lobortis tempor. Donec quam eros, faucibus eu tincidunt vitae, maximus a leo. In bibendum dapibus feugiat. Pellentesque ut urna ante. Phasellus metus lectus, consequat ac urna non, eleifend tempor sem. Vivamus eu elit elit. Sed ac velit mauris. Praesent varius ipsum ex, nec dictum justo accumsan eu. Ut accumsan felis eu mauris egestas, nec tempus dui tempor. Phasellus ut nibh placerat, iaculis dui ac, scelerisque metus. Suspendisse potenti.</p>
                <p>Etiam suscipit nisi vitae diam lacinia, sed euismod dolor varius. Pellentesque id dolor quis eros fringilla ultricies. Donec nec placerat arcu, eu molestie tortor. Quisque lacinia egestas congue. Etiam maximus eu urna eget tempus. Integer tincidunt at augue egestas elementum. Integer pretium, metus at tristique viverra, elit mauris porttitor lectus, at pretium augue nunc nec tortor. Vestibulum cursus mauris massa, eu tristique ligula bibendum vitae.</p>
              </td>
            </tr>
          </tbody>
        </table>
      </div>
    </div>
  </div>
</template>

<script>
export default {
  name: "ProjectPage",
  props: ["projects"]
};
</script>