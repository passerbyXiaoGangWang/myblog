package controllers

import (
	"github.com/astaxie/beego"
)

type MainController struct {
	beego.Controller
}

func (c *MainController) Get() {
	c.Data["Website"] = "beego.me"
	c.Data["Email"] = "astaxie@gmail.com"
	c.TplName = "index.tpl"

	type User struct {
		Name string
		Age int
		Sex string
	}
	u := &User{
		"Joe",
		18,
		"male"}
	c.Data["User"] 	=u

	nums := []int{1,2,3,4,5,6,7,8,9,0}
	c.Data["Nums"] =nums

	c.Data["TplVar"] ="hey guys"

	c.Data["Html"] ="<div>hello beego</div>"

}
