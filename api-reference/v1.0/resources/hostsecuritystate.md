---
title: tipo de recurso de hostSecurityState
description: Contém informações de estado sobre o host (incluindo dispositivos, computadores e assim por diante).
ms.openlocfilehash: 3649553ae0f96222a09825e8819dfd0d199f8454
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/29/2018
ms.locfileid: "27006227"
---
# <a name="hostsecuritystate-resource-type"></a>tipo de recurso de hostSecurityState

Contém informações de estado sobre o host (incluindo dispositivos, computadores e assim por diante).

## <a name="properties"></a>Propriedades

| Propriedade   | Tipo|Descrição|
|:---------------|:--------|:----------|
|FQDN|String|FQDN (nome de domínio totalmente qualificado) do host (por exemplo, `machine.company.com`).|
|isAzureAadJoined|Booliano|True se o host está integrado aos serviços de domínio do Azure Active Directory ao domínio.|
|isAzureAadRegistered|Booliano|True se o host registrado com o Windows Azure Active Directory dispositivo registro (BYOD dispositivos - ou seja, não totalmente gerenciados pelo enterprise).|
|isHybridAzureDomainJoined|Booliano|True se o host é associado a um domínio do Active Directory no local de domínio.|
|Nome_netbios|String|O nome de host local, sem o nome de domínio DNS.|
|sistema operacional|String|Sistema operacional do host. (Por exemplo, Windows10, MacOS, RHEL, etc.).|
|privateIpAddress|String|Endereço IPv4 ou IPv6 (não pode ser roteado) particular (consulte [RFC 1918](https://tools.ietf.org/html/rfc1918)) no momento do alerta.|
|publicIpAddress|String|Endereço IPv4 ou IPv6 roteável publicamente (consulte [RFC 1918](https://tools.ietf.org/html/rfc1918)) em tempo de alerta.|
|riskScore|String|Pontuação de risco de provedor-gerado/calculado do host.  Valor recomendado o intervalo de 0-1, que é igual a um percentual.|

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
