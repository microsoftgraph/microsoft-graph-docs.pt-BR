---
title: Tipo de recurso hostSecurityState
description: " > **Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e sujeitas a alterações. Não há suporte para o uso dessas APIs em aplicativos de produção."
ms.localizationpriority: medium
doc_type: resourcePageType
ms.prod: security
author: preetikr
ms.openlocfilehash: 55a947e26b8ebb147ac0ef52d5764435846d30ea
ms.sourcegitcommit: 95df356bd43b8e5f60fb4c2b62bfa0d5f36a61c2
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/04/2022
ms.locfileid: "65899642"
---
# <a name="hostsecuritystate-resource-type"></a>Tipo de recurso hostSecurityState

Namespace: microsoft.graph

 [!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Contém informações com estado sobre o host (incluindo dispositivos, computadores e assim por diante).

## <a name="properties"></a>Propriedades

| Propriedade   | Tipo|Descrição|
|:---------------|:--------|:----------|
|Fqdn|Cadeia de Caracteres|FQDN do host (nome de domínio totalmente qualificado) (por exemplo, machine.company.com).|
|isAzureAadJoined|Booliano|True se o host for ingressado no domínio para o Azure Active Directory Domain Services.|
|isAzureAadRegistered|Booliano|True se o host registrado com o Registro de Dispositivo do Azure Active Directory (dispositivos BYOD – ou seja, não totalmente gerenciado pela empresa).|
|isHybridAzureDomainJoined|Booliano|True se o host for ingressado no domínio em um domínio do Active Directory local.|
|netBiosName|Cadeia de Caracteres|O nome do host local, sem o nome de domínio DNS.|
|os|String|Sistema operacional do host. (Por exemplo, Windows10, MacOS, RHEL etc.).|
|privateIpAddress|Cadeia de Caracteres|Endereço IPv4 ou IPv6 privado (não roteável) (consulte [RFC 1918](https://tools.ietf.org/html/rfc1918)) no momento do alerta.|
|publicIpAddress|Cadeia de Caracteres|Endereço IPv4 ou IPv6 roteável publicamente (consulte [RFC 1918](https://tools.ietf.org/html/rfc1918)) no momento do alerta.|
|riskScore|Cadeia de Caracteres|Pontuação de risco calculada/gerada pelo provedor do host.  Intervalo de valor recomendado de 0 a 1, que equivale a um percentual.|

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


