---
title: Tipo de recurso pfxRecryptionRequest
description: Ainda não documentado
author: dougeby
ms.localizationpriority: medium
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 7accd07576b93448268eed950768b02a57eceb68
ms.sourcegitcommit: 6c04234af08efce558e9bf926062b4686a84f1b2
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/12/2021
ms.locfileid: "59074847"
---
# <a name="pfxrecryptionrequest-resource-type"></a>Tipo de recurso pfxRecryptionRequest

Namespace: microsoft.graph

> **Importante:** As APIs Graph Microsoft na versão /beta estão sujeitas a alterações; não há suporte para uso de produção.

> **Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.

Ainda não documentado

## <a name="methods"></a>Métodos
|Método|Tipo de retorno|Descrição|
|:---|:---|:---|
|[Listar pfxRecryptionRequests](../api/intune-raimportcerts-pfxrecryptionrequest-list.md)|[Coleção pfxRecryptionRequest](../resources/intune-raimportcerts-pfxrecryptionrequest.md)|Listar propriedades e relações dos objetos [pfxRecryptionRequest.](../resources/intune-raimportcerts-pfxrecryptionrequest.md)|
|[Obter pfxRecryptionRequest](../api/intune-raimportcerts-pfxrecryptionrequest-get.md)|[pfxRecryptionRequest](../resources/intune-raimportcerts-pfxrecryptionrequest.md)|Leia propriedades e relações do objeto [pfxRecryptionRequest.](../resources/intune-raimportcerts-pfxrecryptionrequest.md)|
|[Criar pfxRecryptionRequest](../api/intune-raimportcerts-pfxrecryptionrequest-create.md)|[pfxRecryptionRequest](../resources/intune-raimportcerts-pfxrecryptionrequest.md)|Crie um novo [objeto pfxRecryptionRequest.](../resources/intune-raimportcerts-pfxrecryptionrequest.md)|
|[Excluir pfxRecryptionRequest](../api/intune-raimportcerts-pfxrecryptionrequest-delete.md)|Nenhum|Exclui um [pfxRecryptionRequest](../resources/intune-raimportcerts-pfxrecryptionrequest.md).|
|[Atualizar pfxRecryptionRequest](../api/intune-raimportcerts-pfxrecryptionrequest-update.md)|[pfxRecryptionRequest](../resources/intune-raimportcerts-pfxrecryptionrequest.md)|Atualize as propriedades de um [objeto pfxRecryptionRequest.](../resources/intune-raimportcerts-pfxrecryptionrequest.md)|

## <a name="properties"></a>Propriedades
|Propriedade|Tipo|Descrição|
|:---|:---|:---|
|tenantId|Guid|Ainda não documentado|
|userId|Guid|Ainda não documentado|
|deviceId|Guid|Ainda não documentado|
|profileId|Guid|Ainda não documentado|
|thumbprint|String|Ainda não documentado|
|deviceKeyThumbprint|String|Ainda não documentado|
|status|Int32|Ainda não documentado|
|sourceType|Int32|Ainda não documentado|
|createdTime|DateTimeOffset|Ainda não documentado|
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



