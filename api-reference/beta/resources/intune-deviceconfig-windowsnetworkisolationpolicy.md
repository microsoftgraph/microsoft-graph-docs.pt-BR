---
title: Tipo de recurso windowsNetworkIsolationPolicy
description: Windows Política de Isolamento de Rede
author: dougeby
ms.localizationpriority: medium
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 7836c32467f11be89fd8c2ce1a1c5d46875959bd
ms.sourcegitcommit: 6c04234af08efce558e9bf926062b4686a84f1b2
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/12/2021
ms.locfileid: "59147889"
---
# <a name="windowsnetworkisolationpolicy-resource-type"></a>Tipo de recurso windowsNetworkIsolationPolicy

Namespace: microsoft.graph

> **Importante:** As APIs Graph Microsoft na versão /beta estão sujeitas a alterações; não há suporte para uso de produção.

> **Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.

Windows Política de Isolamento de Rede

## <a name="properties"></a>Propriedades
|Propriedade|Tipo|Descrição|
|:---|:---|:---|
|enterpriseNetworkDomainNames|String collection|Esta é a lista dos domínios que compõem os limites da empresa. Os dados de um desses domínios enviados a um dispositivo serão considerados dados corporativos e protegidos. Esses locais serão considerados um destino seguro para os dados corporativos a serem compartilhados.|
|enterpriseCloudResources|Coleção [proxiedDomain](../resources/intune-shared-proxieddomain.md)|Contém uma lista de domínios de recursos corporativos hospedados na nuvem que precisam ser protegidos. As conexões com esses recursos são consideradas dados corporativos. Se um proxy for emparelhado com um recurso de nuvem, o tráfego para esse recurso será roteado pela rede da empresa por meio do servidor proxy indicado (na porta 80). Um servidor proxy usado para essa finalidade também deve ser configurado usando a política EnterpriseInternalProxyServers. Esta coleção pode conter um máximo de 500 elementos.|
|enterpriseIPRanges|Coleção [ipRange](../resources/intune-shared-iprange.md)|Define os intervalos IP da empresa que definem os computadores da rede corporativa. Dados provenientes desses computadores serão considerados parte da empresa e serão protegidos. Esses locais serão considerados um destino seguro para os dados corporativos a serem compartilhados. Esta coleção pode conter um máximo de 500 elementos.|
|enterpriseInternalProxyServers|String collection|Esta é a lista separada por vírgula de servidores proxy internos. Por exemplo, "157.54.14.28, 157.54.11.118, 10.202.14.167, 157.53.14.163, 157.69.210.59". Esses proxies foram configurados pelo administrador para se conectarem a recursos específicos na Internet. Eles são considerados locais de rede da empresa. Os proxies só são aproveitados na configuração da política EnterpriseCloudResources para forçar o tráfego para os recursos de nuvem corresponderem por meio desses proxies.|
|enterpriseIPRangesAreAuthoritative|Boolean|Valor booliano que informa ao cliente para aceitar a lista configurada e não usar heurística para tentar localizar outras sub-redes. O padrão é falso.|
|enterpriseProxyServers|String collection|Esta é uma lista de servidores proxy. Qualquer servidor que não está nessa lista é considerado não empresarial.|
|enterpriseProxyServersAreAuthoritative|Boolean|Valor booliano que informa ao cliente para aceitar a lista configurada de proxies e não tentar detectar outros proxies de trabalho. O padrão é false|
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
      "@odata.type": "microsoft.graph.ipRange"
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



