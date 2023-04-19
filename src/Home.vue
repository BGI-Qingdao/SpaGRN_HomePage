<template>
    <div class='background'>
        <div class='center-div'>
            <el-row id='header-col1' > <!-- Title of page -->
                <el-col  :span="24"><h1>SpaGRN&#58; GRN inference for SRT data</h1></el-col>
            </el-row>
            <hr>
            <el-tabs v-model="activeName" type="border-card" > <!-- The main menu -->
                <el-tab-pane label="Atlases" name="atlas"> <!-- The Atlas panel -->
                    <el-row> <!-- The first row of database -->
                        <el-col :span="18">  <!-- The friutfly section -->
                            <el-row> <!-- section header -->
                                <el-col :span="24"> 
                                    <h2>Developing Fruit Fly (<i>drosophila</i>) Embryos and Larvae</h2>
                                </el-col>
                            </el-row>
                            <el-row> <!-- The first row dataset  -->
                                <el-col :span="8">  <!-- The E14-16h card-->
                                    <div class='card'>
                                        <el-row> <!-- card name -->
                                            <el-col :span="24">
                                                <h3>E14-16h embryo</h3>
                                            </el-col>
                                        </el-row>
                                        <el-row> <!-- card image -->
                                            <el-col :span="24">
                                                <img src="./assets/E14.png" class="image" >
                                            </el-col>
                                        </el-row>
                                        <el-row> <!-- card buttons -->
                                            <el-col :span="12">
                                                <h3><a href="/SpaGRN/E14_16h_spatial_aware/index.html?atlas=/SpaGRN/E14_16h_spatial_aware" target="_blank">spatial_aware</a></h3>
                                            </el-col>
                                            <el-col :span="12">
                                                <h3><a href="/SpaGRN/E14_16h_spatial_graph/index.html?atlas=/SpaGRN/E14_16h_spatial_graph" target="_blank">spatial_graph</a></h3>
                                            </el-col>
                                        </el-row>
                                        <el-row> <!-- card buttons -->
                                            <el-col :span="24">
                                                <h3><a href="/SpaGRN/E14_16h_pySCENIC/index.html?atlas=/SpaGRN/E14_16h_pySCENIC" target="_blank">pySCENIC</a></h3>
                                            </el-col>
                                        </el-row>
                                    </div>
                                </el-col>
                                <el-col :span="8">  <!-- The E16-18h card-->
                                    <div class='card'>
                                        <el-row> <!-- card name -->
                                            <el-col :span="24">
                                                <h3>E16-18h embryo</h3>
                                            </el-col>
                                        </el-row>
                                        <el-row> <!-- card image -->
                                            <el-col :span="24">
                                                <img src="./assets/E16.png" class="image" >
                                            </el-col>
                                        </el-row>
                                        <el-row> <!-- card buttons -->
                                            <el-col :span="12">
                                                <h3><a href="/SpaGRN/E16_18h_spatial_aware/index.html?atlas=/SpaGRN/E16_18h_spatial_aware" target="_blank">spatial_aware</a></h3>
                                            </el-col>
                                            <el-col :span="12">
                                                <h3><a href="/SpaGRN/E16_18h_spatial_graph/index.html?atlas=/SpaGRN/E16_18h_spatial_graph" target="_blank">spatial_graph</a></h3>
                                            </el-col>
                                        </el-row>
                                        <el-row> <!-- card buttons -->
                                            <el-col :span="24">
                                                <h3><a href="/SpaGRN/E16_18h_pySCENIC/index.html?atlas=/SpaGRN/E16_18h_pySCENIC" target="_blank">pySCENIC</a></h3>
                                            </el-col>
                                        </el-row>
                                    </div>
                                </el-col>
                                <el-col :span="8">  <!-- The L1 card-->
                                    <div class='card'>
                                        <el-row> <!-- card name -->
                                            <el-col :span="24">
                                                <h3>L1 larva</h3>
                                            </el-col>
                                        </el-row>
                                        <el-row> <!-- card image -->
                                            <el-col :span="24">
                                                <img src="./assets/L1.png" class="image" >
                                            </el-col>
                                        </el-row>
                                        <el-row> <!-- card buttons -->
                                            <el-col :span="12">
                                                <h3><a href="/SpaGRN/L1_spatial_aware/index.html?atlas=/SpaGRN/L1_spatial_aware" target="_blank">spatial_aware</a></h3>
                                            </el-col>
                                            <el-col :span="12">
                                                <h3><a href="/SpaGRN/L1_spatial_graph/index.html?atlas=/SpaGRN/L1_spatial_graph" target="_blank">spatial_graph</a></h3>
                                            </el-col>
                                        </el-row>
                                        <el-row> <!-- card buttons -->
                                            <el-col :span="24">
                                                <h3><a href="/SpaGRN/L1_pySCENIC/index.html?atlas=/SpaGRN/L1_pySCENIC" target="_blank">pySCENIC</a></h3>
                                            </el-col>
                                        </el-row>
                                    </div>
                                </el-col>
                            </el-row>
                            <el-row> <!-- The second row dataset  -->
                                <el-col :span="12">  <!-- The L2 card-->
                                    <div class='card'>
                                        <el-row> <!-- card name -->
                                            <el-col :span="24">
                                                <h3>L2 larva</h3>
                                            </el-col>
                                        </el-row>
                                        <el-row> <!-- card image -->
                                            <el-col :span="24">
                                                <img src="./assets/L2.png" class="image" >
                                            </el-col>
                                        </el-row>
                                        <el-row> <!-- card buttons -->
                                            <el-col :span="8">
                                                <h3><a href="/SpaGRN/L2_pySCENIC/index.html?atlas=/SpaGRN/L2_pySCENIC" target="_blank">pySCENIC</a></h3>
                                            </el-col>
                                            <el-col :span="8">
                                                <h3><a href="/SpaGRN/L2_spatial_aware/index.html?atlas=/SpaGRN/L2_spatial_aware" target="_blank">spatial_aware</a></h3>
                                            </el-col>
                                            <el-col :span="8">
                                                <h3><a href="/SpaGRN/L2_spatial_graph/index.html?atlas=/SpaGRN/L2_spatial_graph" target="_blank">spatial_graph</a></h3>
                                            </el-col>
                                        </el-row>
                                    </div>
                                </el-col>
                                <el-col :span="12">  <!-- The L3 card-->
                                    <div class='card'>
                                        <el-row> <!-- card name -->
                                            <el-col :span="24">
                                                <h3>L3 larva</h3>
                                            </el-col>
                                        </el-row>
                                        <el-row> <!-- card image -->
                                            <el-col :span="24">
                                                <img src="./assets/L3.png" class="image" >
                                            </el-col>
                                        </el-row>
                                        <el-row> <!-- card buttons -->
                                            <el-col :span="8">
                                                <h3><a href="/SpaGRN/L3_pySCENIC/index.html?atlas=/SpaGRN/L3_pySCENIC" target="_blank">pySCENIC</a></h3>
                                            </el-col>
                                            <el-col :span="8">
                                                <h3><a href="/SpaGRN/L3_spatial_aware/index.html?atlas=/SpaGRN/L3_spatial_aware" target="_blank">spatial_aware</a></h3>
                                            </el-col>
                                            <el-col :span="8">
                                                <h3><a href="/SpaGRN/L3_spatial_graph/index.html?atlas=/SpaGRN/L3_spatial_graph" target="_blank">spatial_graph</a></h3>
                                            </el-col>
                                        </el-row>
                                    </div>
                                </el-col>
                            </el-row>
                        </el-col>
                        <el-col :span="6">  <!-- The right section -->
                            <el-row> <!-- the mousebrain dataset -->
                                <el-col :span="24">
                                    <h2>More 2D dataset</h2>
                                    <div class='card'>
                                        <el-row> <!-- card name -->
                                            <el-col :span="24">
                                                <h3>Mouse brain data</h3>
                                            </el-col>
                                        </el-row>
                                        <el-row> <!-- card image -->
                                            <el-col :span="24">
                                                <img src="./assets/mousebrain.png" class="image" >
                                            </el-col>
                                        </el-row>
                                        <el-row> <!-- card buttons -->
                                            <el-col :span="12">
                                                <h3><a href="/SpaGRN/mousebrain_spatial_aware/index.html?atlas=/SpaGRN/mousebrain_spatial_aware" target="_blank">spatial_aware</a></h3>
                                            </el-col>
                                            <el-col :span="12">
                                                <h3><a href="/SpaGRN/mousebrain_spatial_graph/index.html?atlas=/SpaGRN/mousebrain_spatial_graph" target="_blank">spatial_graph</a></h3>
                                            </el-col>
                                        </el-row>
                                        <el-row> <!-- card buttons -->
                                            <el-col :span="24">
                                                <h3><a href="/SpaGRN/mousebrain_pySCENIC/index.html?atlas=/SpaGRN/mousebrain_pySCENIC" target="_blank">pySCENIC</a></h3>
                                            </el-col>
                                        </el-row>
                                    </div>
                                </el-col>
                            </el-row>
                        </el-col>
                    </el-row>
                </el-tab-pane>
                <el-tab-pane label="Resources" name='data'> <!-- The download panel -->
                    <h3>Dataset description and data download&#58;</h3> <!-- panel title -->
                    <el-row> <!-- table header -->
                        <el-col :span="6"><h4>name</h4></el-col>
                        <el-col :span="6"><h4>input h5ad data</h4></el-col>
                        <el-col :span="6"><h4>input TF database</h4></el-col>
                        <el-col :span="6"><h4>reference</h4></el-col>
                    </el-row>
                    <el-row> <!-- row of fruitfly -->
                        <el-col :span="6"><h5>Developing fruit fly (<i>drosophila</i>) embryos and larvae data</h5></el-col>
                        <el-col :span="6">
                            <el-row>
                                <el-col :span="24">
                                    <h5><a href="/SpaGRN/fly3d_E14_16h.h5ad" target="_blank">fly3d_L4_16h.h5ad</a></h5> 
                                </el-col>
                                <el-col :span="24">
                                    <h5><a href="/SpaGRN/fly3d_E16_18h.h5ad" target="_blank">fly3d_L6_18h.h5ad</a></h5> 
                                </el-col>
                                <el-col :span="24">
                                    <h5><a href="/SpaGRN/fly3d_L1.h5ad" target="_blank">fly3d_L1.h5ad</a></h5> 
                                </el-col>
                                <el-col :span="24">
                                    <h5><a href="/SpaGRN/fly3d_L2.h5ad" target="_blank">fly3d_L2.h5ad</a></h5> 
                                </el-col>
                                <el-col :span="24">
                                    <h5><a href="/SpaGRN/fly3d_L3.h5ad" target="_blank">fly3d_L3.h5ad</a></h5> 
                                </el-col>
                            </el-row>
                        </el-col>
                        <el-col :span="6">
                            <el-row>
                                <el-col :span="24">
                                    <h5><a href="/SpaGRN/fruitfly.tar.gz" target="_blank">fruitfly.tar.gz</a></h5>
                                </el-col>
                            </el-row>
                        </el-col>
                       <el-col :span="6">
                         <h5><a href="https://doi.org/10.1016/j.devcel.2022.04.006" target="_blank">Wang et al., Developmental Cell, 2022 High-resolution 3D spatiotemporal transcriptomic maps of developing Drosophila embryos and larvae </a></h5>
                       </el-col>
                    </el-row>
                    <el-row> <!-- row of mousebrain -->
                        <el-col :span="6"><h5>Mouse brain data</h5></el-col>
                        <el-col :span="6">
                            <el-row>
                                <el-col :span="24">
                                    <h5><a href="/SpaGRN/mousebrain.h5ad" target="_blank">mousebrain.h5ad</a></h5> 
                                </el-col>
                            </el-row>
                        </el-col>
                        <el-col :span="6">
                            <el-row>
                                <el-col :span="24">
                                    <h5><a href="/SpaGRN/mousebrain.tar.gz" target="_blank">mousebrain.tar.gz</a></h5>
                                </el-col>
                            </el-row>
                        </el-col>
                       <el-col :span="6">
                         <h5><a href="https://doi.org/10.1016/j.cell.2022.04.003" target="_blank">Chen et al., Cell, 2022 Spatiotemporal transcriptomic atlas of mouse organogenesis using DNA nanoball-patterned arrays</a></h5>
                       </el-col>
                    </el-row>
                    <br>
                    <h3>Source codes&#58;</h3>
                    <el-row>
                        <el-col :span="12">
                            <a href="https://github.com/BGI-Qingdao/SpaGRN" target="_blank">Source codes of SpaGRN in GitHub</a><br>
                        </el-col>
                        <el-col :span="12">
                            <a href="https://github.com/BGI-Qingdao/SpaGRN_HomePage" target="_blank">Source codes of this homepage in GitHub</a>
                        </el-col>
                    </el-row>
                </el-tab-pane>
            </el-tabs>
            <hr>
            <div class='footer'>
                <el-row>
                    <el-col :span="3">
                        <img src="./assets/bgi.png" class="logo" >
                    </el-col>
                    <el-col :span="3">
                        <img src="./assets/bgi_research.png" class="logo" >
                    </el-col>
                    <el-col :span="3">
                        <img src="./assets/stomics.png" class="logo" >
                    </el-col>
                    <el-col :span="3">
                        <img src="./assets/stomicsdb.png" class="logo" >
                    </el-col>
                    <el-col :span="3">
                        <img src="./assets/cngb.png" class="logo" >
                    </el-col>
                    <el-col :span="9">
                        <p>For any inquiries about the website, please contact: guolidong@genomics.cn; liyao1@genomics.cn</p>
                        <p>Powered by Element.js and Echarts.js</p>
                    </el-col>
                </el-row>
                <el-row>
                    <el-col :span="24">
                        <p>Copyright &#169; All Rights Reserved 2023 BGI Research <a href=https://beian.miit.gov.cn/>鲁ICP备2022034375号</a></p>
                    </el-col>
                </el-row>
            </div>
        </div>
    </div>
</template>

<script>
export default {
    data() {
        return {
          tid: '1',
          activeName: 'atlas',
        }
    },
};
</script>

<style>
  #header-col1 {
    background-color: #4381e6;
    text-align: center;
    line-height: 100px;
    font-weight: bold;
    color: white;
  }
  .logo{
    width: 100%;
    display: block;
    margin:10px;
    padding:20px;
  }
  .footer{
    border-color: #eeeeee;
    border-style: solid;
    border-width: 1px;
    color: #8b8c8f;
    font-size: 14px;
    padding:10px;
  }
  .image {
    width: 100%;
    display: block;
  }
  .card{
     border-width: 2px;
     border-style: solid;
     border-color:#111111;
     margin:10px
  }
  .tutorial{
     background-color: #ccc;
     border-width: 2px;
     border-style: dashed;
     border-color:#111111;
     text-align: left;
     margin:10px;
     padding:10px;
  }
  .left_border{
     border-left: 3px dashed gray;
  }
  .upper_border{
     border-top: 3px dashed gray;
  }
  .center-div
  {
    margin: 0 auto;
    width: 1300px;
    background-color: white;
    padding:5px;
  }
  .background
  {
      background-color: #ccc;
  }
</style>
