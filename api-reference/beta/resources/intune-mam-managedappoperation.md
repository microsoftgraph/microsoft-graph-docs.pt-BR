---
title: Tipo de recurso managedAppOperation
description: Representa uma operação aplicada a um registro de aplicativo.
author: rolyon
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: c09b823fba3c32ccb4f2950233e9cfa388ff35ba
ms.sourcegitcommit: 94aaf594c881c02f353c6a417460cdf783a0bfe0
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/11/2019
ms.locfileid: "33940747"
---
# <a name="managedappoperation-resource-type"></a>Tipo de recurso managedAppOperation

> **Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.

> **Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.

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
|displayName|Cadeia de caracteres|O nome da operação.|
|lastModifiedDateTime|DateTimeOffset|Última vez em que a operação de aplicativo foi modificada.|
|state|String|O estado atual da operação|
|id|Cadeia de caracteres|Chave da entidade.|
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




