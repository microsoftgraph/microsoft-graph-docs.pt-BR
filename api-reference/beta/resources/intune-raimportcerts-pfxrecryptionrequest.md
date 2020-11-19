---
title: tipo de recurso pfxRecryptionRequest
description: Ainda não documentado
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 904ce75ba1b3afb135ba2788dcde4c629c34a2ff
ms.sourcegitcommit: eb536655ffd8d49ae258664f35c50a8263238400
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/18/2020
ms.locfileid: "49307161"
---
# <a name="pfxrecryptionrequest-resource-type"></a>tipo de recurso pfxRecryptionRequest

Namespace: microsoft.graph

> **Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.

> **Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.

Ainda não documentado

## <a name="methods"></a>Métodos
|Método|Tipo de retorno|Descrição|
|:---|:---|:---|
|[Listar pfxRecryptionRequests](../api/intune-raimportcerts-pfxrecryptionrequest-list.md)|coleção [pfxRecryptionRequest](../resources/intune-raimportcerts-pfxrecryptionrequest.md)|Listar Propriedades e relações dos objetos [pfxRecryptionRequest](../resources/intune-raimportcerts-pfxrecryptionrequest.md) .|
|[Obter pfxRecryptionRequest](../api/intune-raimportcerts-pfxrecryptionrequest-get.md)|[pfxRecryptionRequest](../resources/intune-raimportcerts-pfxrecryptionrequest.md)|Leia as propriedades e as relações do objeto [pfxRecryptionRequest](../resources/intune-raimportcerts-pfxrecryptionrequest.md) .|
|[Criar pfxRecryptionRequest](../api/intune-raimportcerts-pfxrecryptionrequest-create.md)|[pfxRecryptionRequest](../resources/intune-raimportcerts-pfxrecryptionrequest.md)|Criar um novo objeto [pfxRecryptionRequest](../resources/intune-raimportcerts-pfxrecryptionrequest.md) .|
|[Excluir pfxRecryptionRequest](../api/intune-raimportcerts-pfxrecryptionrequest-delete.md)|Nenhum|Exclui [pfxRecryptionRequest](../resources/intune-raimportcerts-pfxrecryptionrequest.md).|
|[Atualizar pfxRecryptionRequest](../api/intune-raimportcerts-pfxrecryptionrequest-update.md)|[pfxRecryptionRequest](../resources/intune-raimportcerts-pfxrecryptionrequest.md)|Atualiza as propriedades de um objeto [pfxRecryptionRequest](../resources/intune-raimportcerts-pfxrecryptionrequest.md) .|

## <a name="properties"></a>Propriedades
|Propriedade|Tipo|Descrição|
|:---|:---|:---|
|tenantId|Guid|Ainda não documentado|
|userId|Guid|Ainda não documentado|
|deviceId|Guid|Ainda não documentado|
|ProfileId|Guid|Ainda não documentado|
|identificação|String|Ainda não documentado|
|deviceKeyThumbprint|String|Ainda não documentado|
|status|Int32|Ainda não documentado|
|sourceType|Int32|Ainda não documentado|
|createdtime|DateTimeOffset|Ainda não documentado|
|lastModifiedTime|DateTimeOffset|Ainda não documentado|
|isDeleted|Booliano|Ainda não documentado|
|eTag|String|Ainda não documentado|

## <a name="relationships"></a>Relações
Nenhum

## <a name="json-representation"></a>Representação JSON
Veja a seguir uma representação JSON do recurso.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.pfxRecryptionRequest"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.pfxRecryptionRequest",
  "tenantId": "Guid",
  "userId": "Guid",
  "deviceId": "Guid",
  "profileId": "Guid",
  "thumbprint": "String",
  "deviceKeyThumbprint": "String",
  "status": 1024,
  "sourceType": 1024,
  "createdTime": "String (timestamp)",
  "lastModifiedTime": "String (timestamp)",
  "isDeleted": true,
  "eTag": "String"
}
```




