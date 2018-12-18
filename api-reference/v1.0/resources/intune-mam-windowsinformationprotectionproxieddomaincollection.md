---
title: Tipo de recurso windowsInformationProtectionProxiedDomainCollection
description: Coleção de domínios como proxy da Proteção de Informações do Windows
author: tfitzmac
ms.openlocfilehash: c95c54c5bbfcc1b5202a0c56a6e3932b35ffac88
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 12/18/2018
ms.locfileid: "27309468"
---
# <a name="windowsinformationprotectionproxieddomaincollection-resource-type"></a><span data-ttu-id="aca20-103">Tipo de recurso windowsInformationProtectionProxiedDomainCollection</span><span class="sxs-lookup"><span data-stu-id="aca20-103">windowsInformationProtectionProxiedDomainCollection resource type</span></span>

> <span data-ttu-id="aca20-104">**Observação:** O uso das APIs do Microsoft Graph para configurar controles e políticas do Intune ainda exige que o serviço do Intune seja [corretamente licenciado](https://go.microsoft.com/fwlink/?linkid=839381) pelo cliente.</span><span class="sxs-lookup"><span data-stu-id="aca20-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="aca20-105">Coleção de domínios como proxy da Proteção de Informações do Windows</span><span class="sxs-lookup"><span data-stu-id="aca20-105">Windows Information Protection Proxied Domain Collection</span></span>
## <a name="properties"></a><span data-ttu-id="aca20-106">Propriedades</span><span class="sxs-lookup"><span data-stu-id="aca20-106">Properties</span></span>
|<span data-ttu-id="aca20-107">Propriedade</span><span class="sxs-lookup"><span data-stu-id="aca20-107">Property</span></span>|<span data-ttu-id="aca20-108">Tipo</span><span class="sxs-lookup"><span data-stu-id="aca20-108">Type</span></span>|<span data-ttu-id="aca20-109">Descrição</span><span class="sxs-lookup"><span data-stu-id="aca20-109">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="aca20-110">displayName</span><span class="sxs-lookup"><span data-stu-id="aca20-110">displayName</span></span>|<span data-ttu-id="aca20-111">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="aca20-111">String</span></span>|<span data-ttu-id="aca20-112">Nome de exibição</span><span class="sxs-lookup"><span data-stu-id="aca20-112">Display name</span></span>|
|<span data-ttu-id="aca20-113">proxiedDomains</span><span class="sxs-lookup"><span data-stu-id="aca20-113">proxiedDomains</span></span>|<span data-ttu-id="aca20-114">Coleção [proxiedDomain](../resources/intune-mam-proxieddomain.md)</span><span class="sxs-lookup"><span data-stu-id="aca20-114">[proxiedDomain](../resources/intune-mam-proxieddomain.md) collection</span></span>|<span data-ttu-id="aca20-115">Coleção de domínios com proxy</span><span class="sxs-lookup"><span data-stu-id="aca20-115">Collection of proxied domains</span></span>|

## <a name="relationships"></a><span data-ttu-id="aca20-116">Relações</span><span class="sxs-lookup"><span data-stu-id="aca20-116">Relationships</span></span>
<span data-ttu-id="aca20-117">Nenhum</span><span class="sxs-lookup"><span data-stu-id="aca20-117">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="aca20-118">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="aca20-118">JSON Representation</span></span>
<span data-ttu-id="aca20-119">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="aca20-119">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.windowsInformationProtectionProxiedDomainCollection"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.windowsInformationProtectionProxiedDomainCollection",
  "displayName": "String",
  "proxiedDomains": [
    {
      "@odata.type": "microsoft.graph.proxiedDomain",
      "ipAddressOrFQDN": "String",
      "proxy": "String"
    }
  ]
}
```



