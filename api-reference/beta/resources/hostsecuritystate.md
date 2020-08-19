---
title: tipo de recurso hostSecurityState
description: " > **Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e sujeitas a alterações. Não há suporte para o uso dessas APIs em aplicativos de produção."
localization_priority: Normal
doc_type: resourcePageType
ms.prod: ''
author: preetikr
ms.openlocfilehash: 5b50c67dff87121caf225ff7191ea8f377616522
ms.sourcegitcommit: a6d284b3726139f11194aa3d23b8bb79165cc09e
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/19/2020
ms.locfileid: "46807938"
---
# <a name="hostsecuritystate-resource-type"></a>tipo de recurso hostSecurityState

Namespace: microsoft.graph

 [!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Contém informações de estado sobre o host (incluindo dispositivos, computadores e assim por diante).

## <a name="properties"></a>Propriedades

| Propriedade   | Tipo|Descrição|
|:---------------|:--------|:----------|
|FQDN|String|FQDN do host (nome de domínio totalmente qualificado) (por exemplo, machine.company.com).|
|isAzureAadJoined|Booliano|True se o host estiver associado ao domínio nos serviços de domínio do Azure Active Directory.|
|isAzureAadRegistered|Booliano|True se o host registrado no registro de dispositivo do Azure Active Directory (dispositivos BYOD-ou seja, não é totalmente gerenciado pela empresa).|
|isHybridAzureDomainJoined|Booliano|True se o host é membro de um domínio do Active Directory local.|
|NetBiosName|String|O nome do host local, sem o nome de domínio DNS.|
|Opera|String|Sistema operacional host. (Por exemplo, Windows10, MacOS, RHEL, etc.).|
|privateIpAddress|String|Privado (não roteável) endereço IPv4 ou IPv6 (consulte [RFC 1918](https://tools.ietf.org/html/rfc1918)) no momento do alerta.|
|publicIpAddress|String|Endereço IPv4 ou IPv6 roteável publicamente (consulte [RFC 1918](https://tools.ietf.org/html/rfc1918)) no momento do alerta.|
|riskScore|String|Pontuação de risco calculado/gerado pelo provedor do host.  O intervalo de valor recomendado de 0-1, que é igual a uma porcentagem.|

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
<!--
{
  "type": "#page.annotation",
  "description": "hostSecurityState resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->
