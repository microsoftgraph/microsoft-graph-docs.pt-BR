---
title: Tipo de recurso auditActor
description: Uma classe que contém as propriedades para Ator de auditoria.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 77150c7a2b883acc6857cd0866459fb9423dfa6c
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/24/2019
ms.locfileid: "32558325"
---
# <a name="auditactor-resource-type"></a>Tipo de recurso auditActor

> **Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.

> **Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.

Uma classe que contém as propriedades para Ator de auditoria.

## <a name="properties"></a>Propriedades
|Propriedade|Tipo|Descrição|
|:---|:---|:---|
|type|String|Tipo de ator.|
|userPermissions|Conjunto de cadeia de caracteres|Lista de permissões de usuário de quando a auditoria foi executada.|
|ApplicationId|String|ID do aplicativo AAD.|
|applicationDisplayName|String|Nome do aplicativo.|
|userPrincipalName|String|Nome principal do usuário (UPN).|
|servicePrincipalName|String|Nome da entidade de serviço (SPN).|
|ipAddress|String|IPAddress.|
|userId|Cadeia de caracteres|ID do usuário.|

## <a name="relationships"></a>Relações
Nenhum

## <a name="json-representation"></a>Representação JSON
Veja a seguir uma representação JSON do recurso.
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.auditActor"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.auditActor",
  "type": "String",
  "userPermissions": [
    "String"
  ],
  "applicationId": "String",
  "applicationDisplayName": "String",
  "userPrincipalName": "String",
  "servicePrincipalName": "String",
  "ipAddress": "String",
  "userId": "String"
}
```





