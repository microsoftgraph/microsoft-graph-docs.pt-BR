---
title: Tipo de recurso managedAppOperation
description: Representa uma operação aplicada a um registro de aplicativo.
author: dougeby
ms.localizationpriority: medium
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 01036699ccafdc177faa8b9abf2192604cc86766
ms.sourcegitcommit: 6c04234af08efce558e9bf926062b4686a84f1b2
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/12/2021
ms.locfileid: "59142562"
---
# <a name="managedappoperation-resource-type"></a>Tipo de recurso managedAppOperation

Namespace: microsoft.graph

> **Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.

Representa uma operação aplicada a um registro de aplicativo.

## <a name="methods"></a>Métodos
|Método|Tipo de retorno|Descrição|
|:---|:---|:---|
|[Listar managedAppOperations](../api/intune-mam-managedappoperation-list.md)|Conjunto [managedAppOperation](../resources/intune-mam-managedappoperation.md)|Listar propriedades e relações de objetos de [managedAppOperation](../resources/intune-mam-managedappoperation.md).|
|[Obter managedAppOperation](../api/intune-mam-managedappoperation-get.md)|[managedAppOperation](../resources/intune-mam-managedappoperation.md)|Ler propriedades e relações de objetos de [managedAppOperation](../resources/intune-mam-managedappoperation.md).|
|[Criar managedAppOperation](../api/intune-mam-managedappoperation-create.md)|[managedAppOperation](../resources/intune-mam-managedappoperation.md)|Criar um novo objeto de[managedAppOperation](../resources/intune-mam-managedappoperation.md).|
|[Excluir managedAppOperation](../api/intune-mam-managedappoperation-delete.md)|Nenhum|Excluir [managedAppOperation](../resources/intune-mam-managedappoperation.md).|
|[Atualizar managedAppOperation](../api/intune-mam-managedappoperation-update.md)|[managedAppOperation](../resources/intune-mam-managedappoperation.md)|Atualizar as propriedades de um objeto de [managedAppOperation](../resources/intune-mam-managedappoperation.md).|

## <a name="properties"></a>Propriedades
|Propriedade|Tipo|Descrição|
|:---|:---|:---|
|displayName|String|O nome da operação.|
|lastModifiedDateTime|DateTimeOffset|Última vez em que a operação de aplicativo foi modificada.|
|state|String|O estado atual da operação|
|id|String|Chave da entidade.|
|versão|String|Versão da entidade.|

## <a name="relationships"></a>Relações
Nenhum

## <a name="json-representation"></a>Representação JSON
Veja a seguir uma representação JSON do recurso.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.managedAppOperation"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.managedAppOperation",
  "displayName": "String",
  "lastModifiedDateTime": "String (timestamp)",
  "state": "String",
  "id": "String (identifier)",
  "version": "String"
}
```




