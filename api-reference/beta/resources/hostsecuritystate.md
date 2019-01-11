---
title: tipo de recurso de hostSecurityState
description: " > **Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e sujeitas a alterações. Não há suporte para o uso dessas APIs em aplicativos de produção."
localization_priority: Normal
ms.openlocfilehash: 1ae1436dd9771d34c37542eb756f81a4f8f0306a
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/11/2019
ms.locfileid: "27853372"
---
# <a name="hostsecuritystate-resource-type"></a>tipo de recurso de hostSecurityState

 > **Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e sujeitas a alterações. Não há suporte para o uso dessas APIs em aplicativos de produção.

Contém informações de estado sobre o host (incluindo dispositivos, computadores e assim por diante).

## <a name="properties"></a>Propriedades

| Propriedade   | Tipo|Descrição|
|:---------------|:--------|:----------|
|FQDN|Cadeia de caracteres|O FQDN (nome totalmente qualificado) (por exemplo, machine.company.com) do host.|
|isAzureAadJoined|Booliano|True se o host está integrado aos serviços de domínio do Azure Active Directory ao domínio.|
|isAzureAadRegistered|Booliano|True se o host registrado com o Windows Azure Active Directory dispositivo registro (BYOD dispositivos - ou seja, não totalmente gerenciados pelo enterprise).|
|isHybridAzureDomainJoined|Booliano|True se o host é associado a um domínio do Active Directory no local de domínio.|
|Nome_netbios|Cadeia de caracteres|O nome de host local, sem o nome de domínio DNS.|
|sistema operacional|Cadeia de caracteres|Sistema operacional do host. (Por exemplo, Windows10, MacOS, RHEL, etc.).|
|privateIpAddress|Cadeia de caracteres|Endereço IPv4 ou IPv6 (não pode ser roteado) particular (consulte [RFC 1918](https://tools.ietf.org/html/rfc1918)) no momento do alerta.|
|publicIpAddress|Cadeia de caracteres|Endereço IPv4 ou IPv6 roteável publicamente (consulte [RFC 1918](https://tools.ietf.org/html/rfc1918)) em tempo de alerta.|
|riskScore|Cadeia de caracteres|Pontuação de risco de provedor-gerado/calculado do host.  Valor recomendado o intervalo de 0-1, que é igual a um percentual.|

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
