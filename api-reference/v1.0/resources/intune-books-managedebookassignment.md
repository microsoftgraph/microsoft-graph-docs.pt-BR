---
title: Tipo de recurso managedEBookAssignment
description: Contém propriedades usadas para atribuir um livro eletrônico a um grupo.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 545f1d40b852208b06089c520cc96f8da28c5e0a
ms.sourcegitcommit: 13f474d3e71d32a5dfe2efebb351e3a1a5aa9685
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/04/2021
ms.locfileid: "52752382"
---
# <a name="managedebookassignment-resource-type"></a>Tipo de recurso managedEBookAssignment

Namespace: microsoft.graph

> **Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.

Contém propriedades usadas para atribuir um livro eletrônico a um grupo.

## <a name="methods"></a>Methods
|Método|Tipo de retorno|Descrição|
|:---|:---|:---|
|[Listar managedEBookAssignments](../api/intune-books-managedebookassignment-list.md)|Conjunto [managedEBookAssignment](../resources/intune-books-managedebookassignment.md)|Listar propriedades e relações de objetos de [managedEBookAssignment](../resources/intune-books-managedebookassignment.md).|
|[Obter managedEBookAssignment](../api/intune-books-managedebookassignment-get.md)|[managedEBookAssignment](../resources/intune-books-managedebookassignment.md)|Ler propriedades e relações de objetos de [managedEBookAssignment](../resources/intune-books-managedebookassignment.md).|
|[Criar managedEBookAssignment](../api/intune-books-managedebookassignment-create.md)|[managedEBookAssignment](../resources/intune-books-managedebookassignment.md)|Criar um novo objeto de [managedEBookAssignment](../resources/intune-books-managedebookassignment.md).|
|[Excluir managedEBookAssignment](../api/intune-books-managedebookassignment-delete.md)|Nenhum|Excluir [managedEBookAssignment](../resources/intune-books-managedebookassignment.md).|
|[Atualizar managedEBookAssignment](../api/intune-books-managedebookassignment-update.md)|[managedEBookAssignment](../resources/intune-books-managedebookassignment.md)|Atualizar as propriedades de um objeto de [managedEBookAssignment](../resources/intune-books-managedebookassignment.md).|

## <a name="properties"></a>Propriedades
|Propriedade|Tipo|Descrição|
|:---|:---|:---|
|id|Cadeia de caracteres|Chave da entidade.|
|destino|[deviceAndAppManagementAssignmentTarget](../resources/intune-shared-deviceandappmanagementassignmenttarget.md)|O destino da atribuição do livro eletrônico.|
|installIntent|[installIntent](../resources/intune-shared-installintent.md)|A tentativa de instalação do livro eletrônico. Os valores possíveis são: `available`, `required`, `uninstall`, `availableWithoutEnrollment`.|

## <a name="relationships"></a>Relações
Nenhuma

## <a name="json-representation"></a>Representação JSON
Veja a seguir uma representação JSON do recurso.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.managedEBookAssignment"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.managedEBookAssignment",
  "id": "String (identifier)",
  "target": {
    "@odata.type": "microsoft.graph.allLicensedUsersAssignmentTarget"
  },
  "installIntent": "String"
}
```




