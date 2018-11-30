---
title: Tipo de recurso proxiedDomain
description: Domínio com proxy
ms.openlocfilehash: 310ccb1420ed450c9e7c53d534181720f9051ff4
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/29/2018
ms.locfileid: "27034175"
---
# <a name="proxieddomain-resource-type"></a><span data-ttu-id="983a9-103">Tipo de recurso proxiedDomain</span><span class="sxs-lookup"><span data-stu-id="983a9-103">proxiedDomain resource type</span></span>

> <span data-ttu-id="983a9-104">**Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e estão sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="983a9-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="983a9-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="983a9-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="983a9-106">**Observação:** O uso das APIs do Microsoft Graph para configurar controles e políticas do Intune ainda exige que o serviço do Intune seja [corretamente licenciado](https://go.microsoft.com/fwlink/?linkid=839381) pelo cliente.</span><span class="sxs-lookup"><span data-stu-id="983a9-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="983a9-107">Domínio com proxy</span><span class="sxs-lookup"><span data-stu-id="983a9-107">Proxied Domain</span></span>

## <a name="properties"></a><span data-ttu-id="983a9-108">Propriedades</span><span class="sxs-lookup"><span data-stu-id="983a9-108">Properties</span></span>
|<span data-ttu-id="983a9-109">Propriedade</span><span class="sxs-lookup"><span data-stu-id="983a9-109">Property</span></span>|<span data-ttu-id="983a9-110">Tipo</span><span class="sxs-lookup"><span data-stu-id="983a9-110">Type</span></span>|<span data-ttu-id="983a9-111">Descrição</span><span class="sxs-lookup"><span data-stu-id="983a9-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="983a9-112">ipAddressOrFQDN</span><span class="sxs-lookup"><span data-stu-id="983a9-112">ipAddressOrFQDN</span></span>|<span data-ttu-id="983a9-113">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="983a9-113">String</span></span>|<span data-ttu-id="983a9-114">O endereço IP ou o nome de domínio totalmente qualificado (FQDN).</span><span class="sxs-lookup"><span data-stu-id="983a9-114">The IP address or fully qualified domain name (FQDN).</span></span>|
|<span data-ttu-id="983a9-115">proxy</span><span class="sxs-lookup"><span data-stu-id="983a9-115">proxy</span></span>|<span data-ttu-id="983a9-116">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="983a9-116">String</span></span>|<span data-ttu-id="983a9-117">Endereço do proxy IP ou FQDN.</span><span class="sxs-lookup"><span data-stu-id="983a9-117">Proxy IP address or FQDN.</span></span>|

## <a name="relationships"></a><span data-ttu-id="983a9-118">Relações</span><span class="sxs-lookup"><span data-stu-id="983a9-118">Relationships</span></span>
<span data-ttu-id="983a9-119">Nenhum</span><span class="sxs-lookup"><span data-stu-id="983a9-119">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="983a9-120">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="983a9-120">JSON Representation</span></span>
<span data-ttu-id="983a9-121">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="983a9-121">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.proxiedDomain"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.proxiedDomain",
  "ipAddressOrFQDN": "String",
  "proxy": "String"
}
```



