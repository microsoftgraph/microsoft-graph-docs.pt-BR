---
title: tipo de recurso windowsNetworkIsolationPolicy
description: Política de isolamento de rede do Windows
author: dougeby
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: 4816dfab83c286ed9cbe6ae35cd1c9e3339efb63
ms.sourcegitcommit: bbcf074f0be9d5e02f84c290122850cc5968fb1f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/14/2020
ms.locfileid: "43459987"
---
# <a name="windowsnetworkisolationpolicy-resource-type"></a>tipo de recurso windowsNetworkIsolationPolicy

Namespace: microsoft.graph

> **Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.

> **Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.

Política de isolamento de rede do Windows

## <a name="properties"></a>Propriedades
|Propriedade|Tipo|Descrição|
|:---|:---|:---|
|enterpriseNetworkDomainNames|Coleção de cadeias de caracteres|Esta é a lista dos domínios que compõem os limites da empresa. Os dados de um desses domínios enviados para um dispositivo serão considerados dados corporativos e protegidos. Esses locais serão considerados um destino seguro para que os dados corporativos sejam compartilhados.|
|enterpriseCloudResources|Coleção [proxiedDomain](../resources/intune-shared-proxieddomain.md)|Contém uma lista de domínios de recursos da empresa hospedados na nuvem que precisam ser protegidos. As conexões com esses recursos são consideradas dados corporativos. Se um proxy for emparelhado com um recurso de nuvem, o tráfego para esse recurso será roteado pela rede da empresa por meio do servidor proxy indicado (na porta 80). Um servidor proxy usado para essa finalidade também deve ser configurado usando a política EnterpriseInternalProxyServers. Esta coleção pode conter um máximo de 500 elementos.|
|enterpriseIPRanges|Coleção [ipRange](../resources/intune-shared-iprange.md)|Define os intervalos IP da empresa que definem os computadores da rede corporativa. Dados provenientes desses computadores serão considerados parte da empresa e serão protegidos. Esses locais serão considerados um destino seguro para que os dados corporativos sejam compartilhados. Esta coleção pode conter um máximo de 500 elementos.|
|enterpriseInternalProxyServers|Coleção de cadeias de caracteres|Esta é a lista separada por vírgula de servidores proxy internos. Por exemplo, "157.54.14.28, 157.54.11.118, 10.202.14.167, 157.53.14.163, 157.69.210.59". Esses proxies foram configurados pelo administrador para se conectarem a recursos específicos na Internet. Eles são considerados locais de rede da empresa. Os proxies são utilizados apenas na configuração da política EnterpriseCloudResources para forçar o tráfego para os recursos de nuvem correspondentes através desses proxies.|
|enterpriseIPRangesAreAuthoritative|Booliano|Valor booliano que informa ao cliente para aceitar a lista configurada e não usar heurística para tentar localizar outras sub-redes. O padrão é false.|
|enterpriseProxyServers|Coleção de cadeias de caracteres|Esta é uma lista de servidores proxy. Qualquer servidor que não esteja na lista é considerado não corporativo.|
|enterpriseProxyServersAreAuthoritative|Boolean|Valor booliano que informa ao cliente para aceitar a lista configurada de proxies e não tentar detectar outros proxies de trabalho. O padrão é false|
|neutralDomainResources|Coleção de cadeias de caracteres|Lista de nomes de domínio que podem ser usados para trabalho ou recurso pessoal.|

## <a name="relationships"></a>Relações
Nenhum

## <a name="json-representation"></a>Representação JSON
Veja a seguir uma representação JSON do recurso.
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.windowsNetworkIsolationPolicy"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.windowsNetworkIsolationPolicy",
  "enterpriseNetworkDomainNames": [
    "String"
  ],
  "enterpriseCloudResources": [
    {
      "@odata.type": "microsoft.graph.proxiedDomain",
      "ipAddressOrFQDN": "String",
      "proxy": "String"
    }
  ],
  "enterpriseIPRanges": [
    {
      "@odata.type": "microsoft.graph.iPv6Range",
      "lowerAddress": "String",
      "upperAddress": "String"
    }
  ],
  "enterpriseInternalProxyServers": [
    "String"
  ],
  "enterpriseIPRangesAreAuthoritative": true,
  "enterpriseProxyServers": [
    "String"
  ],
  "enterpriseProxyServersAreAuthoritative": true,
  "neutralDomainResources": [
    "String"
  ]
}
```



