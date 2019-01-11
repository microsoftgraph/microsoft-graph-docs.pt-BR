---
title: tipo de recurso de windowsNetworkIsolationPolicy
description: Política de isolamento de rede do Windows
author: tfitzmac
localization_priority: Normal
ms.openlocfilehash: 82026ba4d82b85a0275f83bb729b495e17ff5d5c
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/11/2019
ms.locfileid: "27834611"
---
# <a name="windowsnetworkisolationpolicy-resource-type"></a>tipo de recurso de windowsNetworkIsolationPolicy

> **Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e estão sujeitas a alterações. Não há suporte para o uso dessas APIs em aplicativos de produção.

> **Observação:** O uso das APIs do Microsoft Graph para configurar controles e políticas do Intune ainda exige que o serviço do Intune seja [corretamente licenciado](https://go.microsoft.com/fwlink/?linkid=839381) pelo cliente.

Política de isolamento de rede do Windows
## <a name="properties"></a>Propriedades
|Propriedade|Tipo|Descrição|
|:---|:---|:---|
|enterpriseNetworkDomainNames|String collection|Esta é a lista dos domínios que compõem os limites da empresa. Dados de um desses domínios que será enviada para um dispositivo serão considerados dados corporativos e protegidos. Serão considerados um destino seguro para dados corporativos para serem compartilhadas desses locais.|
|enterpriseCloudResources|Coleção [proxiedDomain](../resources/intune-shared-proxieddomain.md)|Contém uma lista de domínios de recurso da empresa hospedado na nuvem que precisam ser protegidos. As conexões com esses recursos são consideradas dados corporativos. Se um proxy for emparelhado com um recurso de nuvem, o tráfego para esse recurso será roteado pela rede da empresa por meio do servidor proxy indicado (na porta 80). Um servidor proxy usado para essa finalidade também deve ser configurado usando a política de EnterpriseInternalProxyServers. Esta coleção pode conter um máximo de 500 elementos.|
|enterpriseIPRanges|Coleção [ipRange](../resources/intune-shared-iprange.md)|Define os intervalos IP da empresa que definem os computadores da rede corporativa. Dados provenientes desses computadores serão considerados parte da empresa e serão protegidos. Serão considerados um destino seguro para dados corporativos para serem compartilhadas desses locais. Esta coleção pode conter um máximo de 500 elementos.|
|enterpriseInternalProxyServers|String collection|Esta é a lista separada por vírgula de servidores proxy internos. Por exemplo, "157.54.14.28, 157.54.11.118, 10.202.14.167, 157.53.14.163, 157.69.210.59". Esses proxies foram configurados pelo administrador para se conectarem a recursos específicos na Internet. Eles são considerados locais de rede da empresa. Os proxies somente são utilizados na configuração da diretiva de EnterpriseCloudResources para forçar o tráfego para os recursos de nuvem correspondentes por meio desses proxies.|
|enterpriseIPRangesAreAuthoritative|Booliano|Valor booliano que informa ao cliente para aceitar a lista configurada e não usar heurística para tentar localizar outras sub-redes. O padrão é false.|
|enterpriseProxyServers|String collection|Esta é uma lista de servidores proxy. Qualquer servidor não dessa lista é considerado fora da empresa.|
|enterpriseProxyServersAreAuthoritative|Booliano|Valor booliano que informa ao cliente para aceitar a lista configurada de proxies e não tentar detectar outros proxies de trabalho. O padrão é false|
|neutralDomainResources|String collection|Lista de nomes de domínio que podem ser usados para recursos pessoais ou de trabalho.|

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





