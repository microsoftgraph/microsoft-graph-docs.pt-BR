---
title: Tipo de recurso iosVppEBookAssignment
description: Contém propriedades usadas para atribuir um livro eletrônico iOS VPP a um grupo.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: f074b812a565982177873880f713923a36013f1b
ms.sourcegitcommit: dcf237b515e70302aec0d0c490feb1de7a60613e
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/31/2021
ms.locfileid: "58813752"
---
# <a name="iosvppebookassignment-resource-type"></a>Tipo de recurso iosVppEBookAssignment

Namespace: microsoft.graph

> **Importante:** As APIs Graph Microsoft na versão /beta estão sujeitas a alterações; não há suporte para uso de produção.

> **Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.

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
|id|Cadeia de caracteres|Chave da entidade. Herda do [managedEBookAssignment](../resources/intune-books-managedebookassignment.md)|
|destino|[deviceAndAppManagementAssignmentTarget](../resources/intune-shared-deviceandappmanagementassignmenttarget.md)|O destino da atribuição do livro eletrônico. Herda do [managedEBookAssignment](../resources/intune-books-managedebookassignment.md)|
|installIntent|[installIntent](../resources/intune-shared-installintent.md)|A tentativa de instalação do livro eletrônico. Herdado [de managedEBookAssignment](../resources/intune-books-managedebookassignment.md). Os valores possíveis são: `available`, `required`, `uninstall`, `availableWithoutEnrollment`.|

## <a name="relationships"></a>Relações
Nenhum

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
    "@odata.type": "microsoft.graph.deviceAndAppManagementAssignmentTarget",
    "deviceAndAppManagementAssignmentFilterId": "String",
    "deviceAndAppManagementAssignmentFilterType": "String"
  },
  "installIntent": "String"
}
```



