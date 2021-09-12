---
title: Tipo de recurso hostSecurityState
description: Contém informações de estado sobre o host (incluindo dispositivos, computadores e assim por diante).
ms.localizationpriority: medium
author: preetikr
ms.prod: ''
doc_type: resourcePageType
ms.openlocfilehash: 3513342aaadb2eaf80a787b26988ff2a638813ac
ms.sourcegitcommit: 6c04234af08efce558e9bf926062b4686a84f1b2
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/12/2021
ms.locfileid: "59007205"
---
# <a name="hostsecuritystate-resource-type"></a>Tipo de recurso hostSecurityState

Namespace: microsoft.graph

Contém informações de estado sobre o host (incluindo dispositivos, computadores e assim por diante).

## <a name="properties"></a>Propriedades

| Propriedade   | Tipo|Descrição|
|:---------------|:--------|:----------|
|fqdn|String|FQDN do Host (Nome de Domínio Totalmente Qualificado) (por exemplo, `machine.company.com` ).|
|isAzureAadJoined|Boolean|True se o host estiver ingressado no domínio Azure Active Directory Serviços de Domínio.|
|isAzureAadRegistered|Booliano|True se o host registrado com Azure Active Directory registro de dispositivos (dispositivos BYOD - ou seja, não totalmente gerenciado pela empresa).|
|isHybridAzureDomainJoined|Boolean|True se o host for domínio ingressado em um domínio local do Active Directory.|
|netBiosName|Cadeia de caracteres|O nome de host local, sem o nome de domínio DNS.|
|os|String|Host Operating System. (Por exemplo, Windows10, MacOS, RHEL etc.).|
|privateIpAddress|Cadeia de caracteres|Endereço IPv4 ou IPv6 particular (consulte [RFC 1918](https://tools.ietf.org/html/rfc1918)) no momento do alerta.|
|publicIpAddress|Cadeia de caracteres|Endereço IPv4 ou IPv6 publicamente routable (consulte [RFC 1918](https://tools.ietf.org/html/rfc1918)) no momento do alerta.|
|riskScore|Cadeia de caracteres|Pontuação de risco gerada/calculada pelo provedor do host.  Intervalo de valores recomendado de 0 a 1, que equivale a uma porcentagem.|

## <a name="json-representation"></a>Representação JSON

Veja a seguir uma representação JSON do recurso.

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.hostSecurityState"
}-->

```json
{
  "fqdn": "String",
  "isAzureAadJoined": true,
  "isAzureAadRegistered": true,
  "isHybridAzureDomainJoined": true,
  "netBiosName": "String",
  "os": "String",
  "privateIpAddress": "String",
  "publicIpAddress": "String",
  "riskScore": "String"
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "hostSecurityState resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->

