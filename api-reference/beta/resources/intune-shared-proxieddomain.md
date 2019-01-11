---
title: Tipo de recurso proxiedDomain
description: Domínio com proxy
author: tfitzmac
localization_priority: Normal
ms.openlocfilehash: b25d40058f4f79add5875698777e23f658992e05
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/11/2019
ms.locfileid: "27846771"
---
# <a name="proxieddomain-resource-type"></a><span data-ttu-id="a17dd-103">Tipo de recurso proxiedDomain</span><span class="sxs-lookup"><span data-stu-id="a17dd-103">proxiedDomain resource type</span></span>

> <span data-ttu-id="a17dd-104">**Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e estão sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="a17dd-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="a17dd-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="a17dd-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="a17dd-106">**Observação:** O uso das APIs do Microsoft Graph para configurar controles e políticas do Intune ainda exige que o serviço do Intune seja [corretamente licenciado](https://go.microsoft.com/fwlink/?linkid=839381) pelo cliente.</span><span class="sxs-lookup"><span data-stu-id="a17dd-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="a17dd-107">Domínio com proxy</span><span class="sxs-lookup"><span data-stu-id="a17dd-107">Proxied Domain</span></span>

## <a name="properties"></a><span data-ttu-id="a17dd-108">Propriedades</span><span class="sxs-lookup"><span data-stu-id="a17dd-108">Properties</span></span>
|<span data-ttu-id="a17dd-109">Propriedade</span><span class="sxs-lookup"><span data-stu-id="a17dd-109">Property</span></span>|<span data-ttu-id="a17dd-110">Tipo</span><span class="sxs-lookup"><span data-stu-id="a17dd-110">Type</span></span>|<span data-ttu-id="a17dd-111">Descrição</span><span class="sxs-lookup"><span data-stu-id="a17dd-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="a17dd-112">ipAddressOrFQDN</span><span class="sxs-lookup"><span data-stu-id="a17dd-112">ipAddressOrFQDN</span></span>|<span data-ttu-id="a17dd-113">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="a17dd-113">String</span></span>|<span data-ttu-id="a17dd-114">O endereço IP ou o nome de domínio totalmente qualificado (FQDN).</span><span class="sxs-lookup"><span data-stu-id="a17dd-114">The IP address or fully qualified domain name (FQDN).</span></span>|
|<span data-ttu-id="a17dd-115">proxy</span><span class="sxs-lookup"><span data-stu-id="a17dd-115">proxy</span></span>|<span data-ttu-id="a17dd-116">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="a17dd-116">String</span></span>|<span data-ttu-id="a17dd-117">Endereço do proxy IP ou FQDN.</span><span class="sxs-lookup"><span data-stu-id="a17dd-117">Proxy IP address or FQDN.</span></span>|

## <a name="relationships"></a><span data-ttu-id="a17dd-118">Relações</span><span class="sxs-lookup"><span data-stu-id="a17dd-118">Relationships</span></span>
<span data-ttu-id="a17dd-119">Nenhum</span><span class="sxs-lookup"><span data-stu-id="a17dd-119">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="a17dd-120">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="a17dd-120">JSON Representation</span></span>
<span data-ttu-id="a17dd-121">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="a17dd-121">Here is a JSON representation of the resource.</span></span>
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



