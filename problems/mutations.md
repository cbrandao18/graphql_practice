mutation {
  updateWizard(id: 1, name:"Totally Not Harry Potter") {
    id,
    name,
    house {
      name
    },
    patronus {
      form
    }
  }
}

mutation {
  updateWizard(id: 1, patronusId: 2, houseId: 3) {
    id
    name
    house {
        id
        name
    }
    patronus {
        id
        form
    }
  }
}

mutation {
  deleteWizard(id:1){
      name
  }
}