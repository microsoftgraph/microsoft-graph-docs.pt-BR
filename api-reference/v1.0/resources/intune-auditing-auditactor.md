---
title: Tipo de recurso auditActor
description: Uma classe que contém as propriedades para Ator de auditoria.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 1b6c6eadca68c8c41bc13b9aee3dd547ae1f7921
ms.sourcegitcommit: cd8611227a84db21449ab0ad40bedb665dacb9bb
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 10/18/2021
ms.locfileid: "60450056"
---
# <a name="auditactor-resource-type"></a>Tipo de recurso auditActor

Namespace: microsoft.graph

> **Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.

Uma classe que contém as propriedades para Ator de auditoria.

## <a name="properties"></a>Propriedades
|Propriedade|Tipo|Descrição|
|:---|:---|:---|
|type|Cadeia de caracteres|Tipo de ator.|
|userPermissions|Conjunto de cadeia de caracteres|Lista de permissões de usuário de quando a auditoria foi executada.|
|ApplicationId|Cadeia de caracteres|ID do aplicativo AAD.|
|applicationDisplayName|Cadeia de caracteres|Nome do aplicativo.|
|userPrincipalName|Cadeia de caracteres|Nome principal do usuário (UPN).|
|servicePrincipalName|Cadeia de caracteres|Nome da entidade de serviço (SPN).|
|ipAddress|Cadeia de caracteres|IPAddress.|
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



