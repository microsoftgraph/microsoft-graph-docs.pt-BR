---
title: Tipo de recurso iosVppEBookAssignment
description: Contém propriedades usadas para atribuir um livro eletrônico iOS VPP a um grupo.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 4f472714869d92bcaf2af148dd2f591c19c18425
ms.sourcegitcommit: 873b99d9001d1b2af21836e47f15360b08e10a40
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 02/26/2019
ms.locfileid: "30262227"
---
# <a name="iosvppebookassignment-resource-type"></a>Tipo de recurso iosVppEBookAssignment

> **Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.

Contém propriedades usadas para atribuir um livro eletrônico iOS VPP a um grupo.


Herda de [managedEBookAssignment](../resources/intune-books-managedebookassignment.md)

## <a name="methods"></a>Métodos
|Método|Tipo de retorno|Descrição|
|:---|:---|:---|
|[Listar iosVppEBookAssignments](../api/intune-books-iosvppebookassignment-list.md)|Conjunto [iosVppEBookAssignment](../resources/intune-books-iosvppebookassignment.md)|Listar propriedades e relações de objetos de [iosVppEBookAssignment](../resources/intune-books-iosvppebookassignment.md).|
|[Obter iosVppEBookAssignment](../api/intune-books-iosvppebookassignment-get.md)|[iosVppEBookAssignment](../resources/intune-books-iosvppebookassignment.md)|Ler propriedades e relações de objetos de [iosVppEBookAssignment](../resources/intune-books-iosvppebookassignment.md).|
|[Criar iosVppEBookAssignment](../api/intune-books-iosvppebookassignment-create.md)|[iosVppEBookAssignment](../resources/intune-books-iosvppebookassignment.md)|Criar um novo objeto de [iosVppEBookAssignment](../resources/intune-books-iosvppebookassignment.md).|
|[Excluir iosVppEBookAssignment](../api/intune-books-iosvppebookassignment-delete.md)|Nenhum|Excluir [iosVppEBookAssignment](../resources/intune-books-iosvppebookassignment.md).|
|[Atualizar iosVppEBookAssignment](../api/intune-books-iosvppebookassignment-update.md)|[iosVppEBookAssignment](../resources/intune-books-iosvppebookassignment.md)|Atualizar as propriedades de um objeto de [iosVppEBookAssignment](../resources/intune-books-iosvppebookassignment.md).|

## <a name="properties"></a>Propriedades
|Propriedade|Tipo|Descrição|
|:---|:---|:---|
|id|String|Chave da entidade. Herda do [managedEBookAssignment](../resources/intune-books-managedebookassignment.md)|
|destino|[deviceAndAppManagementAssignmentTarget](../resources/intune-shared-deviceandappmanagementassignmenttarget.md)|O destino da atribuição do livro eletrônico. Herda do [managedEBookAssignment](../resources/intune-books-managedebookassignment.md)|
|installIntent|[installIntent](../resources/intune-shared-installintent.md)|A tentativa de instalação do livro eletrônico. Herdado de [managedEBookAssignment](../resources/intune-books-managedebookassignment.md). Os valores possíveis são: `available`, `required`, `uninstall`, `availableWithoutEnrollment`.|

## <a name="relationships"></a>Relações
Nenhuma

## <a name="json-representation"></a>Representação JSON
Veja a seguir uma representação JSON do recurso.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.iosVppEBookAssignment"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.iosVppEBookAssignment",
  "id": "String (identifier)",
  "target": {
    "@odata.type": "microsoft.graph.deviceAndAppManagementAssignmentTarget"
  },
  "installIntent": "String"
}
```



