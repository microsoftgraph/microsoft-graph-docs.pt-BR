---
title: Tipo de recurso managedAppOperation
description: Representa uma operação aplicada a um registro de aplicativo.
author: tfitzmac
localization_priority: Normal
ms.openlocfilehash: 962468c4d1464b827e234b0aac5452bbd0be576a
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/11/2019
ms.locfileid: "27859035"
---
# <a name="managedappoperation-resource-type"></a>Tipo de recurso managedAppOperation

> **Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e estão sujeitas a alterações. Não há suporte para o uso dessas APIs em aplicativos de produção.

> **Observação:** O uso das APIs do Microsoft Graph para configurar controles e políticas do Intune ainda exige que o serviço do Intune seja [corretamente licenciado](https://go.microsoft.com/fwlink/?linkid=839381) pelo cliente.

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
|estado|Cadeia de caracteres|O estado atual da operação|
|id|Cadeia de caracteres|Chave da entidade.|
|version|Cadeia de caracteres|Versão da entidade.|

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





