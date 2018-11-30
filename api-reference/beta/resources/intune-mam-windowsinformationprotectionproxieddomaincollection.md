---
title: Tipo de recurso windowsInformationProtectionProxiedDomainCollection
description: Coleção de domínios como proxy da Proteção de Informações do Windows
ms.openlocfilehash: 07539361d99211f2a787fe538745debf09fa4cf2
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/29/2018
ms.locfileid: "27039097"
---
# <a name="windowsinformationprotectionproxieddomaincollection-resource-type"></a><span data-ttu-id="1b485-103">Tipo de recurso windowsInformationProtectionProxiedDomainCollection</span><span class="sxs-lookup"><span data-stu-id="1b485-103">windowsInformationProtectionProxiedDomainCollection resource type</span></span>

> <span data-ttu-id="1b485-104">**Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e estão sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="1b485-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="1b485-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="1b485-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="1b485-106">**Observação:** O uso das APIs do Microsoft Graph para configurar controles e políticas do Intune ainda exige que o serviço do Intune seja [corretamente licenciado](https://go.microsoft.com/fwlink/?linkid=839381) pelo cliente.</span><span class="sxs-lookup"><span data-stu-id="1b485-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="1b485-107">Coleção de domínios como proxy da Proteção de Informações do Windows</span><span class="sxs-lookup"><span data-stu-id="1b485-107">Windows Information Protection Proxied Domain Collection</span></span>
## <a name="properties"></a><span data-ttu-id="1b485-108">Propriedades</span><span class="sxs-lookup"><span data-stu-id="1b485-108">Properties</span></span>
|<span data-ttu-id="1b485-109">Propriedade</span><span class="sxs-lookup"><span data-stu-id="1b485-109">Property</span></span>|<span data-ttu-id="1b485-110">Tipo</span><span class="sxs-lookup"><span data-stu-id="1b485-110">Type</span></span>|<span data-ttu-id="1b485-111">Descrição</span><span class="sxs-lookup"><span data-stu-id="1b485-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="1b485-112">displayName</span><span class="sxs-lookup"><span data-stu-id="1b485-112">displayName</span></span>|<span data-ttu-id="1b485-113">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="1b485-113">String</span></span>|<span data-ttu-id="1b485-114">Nome de exibição</span><span class="sxs-lookup"><span data-stu-id="1b485-114">Display name</span></span>|
|<span data-ttu-id="1b485-115">proxiedDomains</span><span class="sxs-lookup"><span data-stu-id="1b485-115">proxiedDomains</span></span>|<span data-ttu-id="1b485-116">Coleção [proxiedDomain](../resources/intune-shared-proxieddomain.md)</span><span class="sxs-lookup"><span data-stu-id="1b485-116">[proxiedDomain](../resources/intune-shared-proxieddomain.md) collection</span></span>|<span data-ttu-id="1b485-117">Coleção de domínios com proxy</span><span class="sxs-lookup"><span data-stu-id="1b485-117">Collection of proxied domains</span></span>|

## <a name="relationships"></a><span data-ttu-id="1b485-118">Relações</span><span class="sxs-lookup"><span data-stu-id="1b485-118">Relationships</span></span>
<span data-ttu-id="1b485-119">Nenhum</span><span class="sxs-lookup"><span data-stu-id="1b485-119">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="1b485-120">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="1b485-120">JSON Representation</span></span>
<span data-ttu-id="1b485-121">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="1b485-121">Here is a JSON representation of the resource.</span></span>
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





