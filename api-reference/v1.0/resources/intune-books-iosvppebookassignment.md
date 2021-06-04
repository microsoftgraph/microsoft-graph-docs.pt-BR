---
title: Tipo de recurso iosVppEBookAssignment
description: Contém propriedades usadas para atribuir um livro eletrônico iOS VPP a um grupo.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 6fcc47a65a521658c4cbb97eafd4e90d20f7198f
ms.sourcegitcommit: 13f474d3e71d32a5dfe2efebb351e3a1a5aa9685
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/04/2021
ms.locfileid: "52742920"
---
# <a name="iosvppebookassignment-resource-type"></a>Tipo de recurso iosVppEBookAssignment

Namespace: microsoft.graph

> **Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.

Contém propriedades usadas para atribuir um livro eletrônico iOS VPP a um grupo.


Herda de [managedEBookAssignment](../resources/intune-books-managedebookassignment.md)

## <a name="methods"></a>Methods
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




