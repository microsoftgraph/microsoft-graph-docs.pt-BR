---
title: Tipo de recurso proxiedDomain
description: Domínio com proxy
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: bf4668a58e09b21c2689e10c27e773128f886b34
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/12/2019
ms.locfileid: "27971547"
---
# <a name="proxieddomain-resource-type"></a><span data-ttu-id="a625b-103">Tipo de recurso proxiedDomain</span><span class="sxs-lookup"><span data-stu-id="a625b-103">proxiedDomain resource type</span></span>

> <span data-ttu-id="a625b-104">**Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e estão sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="a625b-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="a625b-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="a625b-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="a625b-106">**Observação:** O uso das APIs do Microsoft Graph para configurar controles e políticas do Intune ainda exige que o serviço do Intune seja [corretamente licenciado](https://go.microsoft.com/fwlink/?linkid=839381) pelo cliente.</span><span class="sxs-lookup"><span data-stu-id="a625b-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="a625b-107">Domínio com proxy</span><span class="sxs-lookup"><span data-stu-id="a625b-107">Proxied Domain</span></span>

## <a name="properties"></a><span data-ttu-id="a625b-108">Propriedades</span><span class="sxs-lookup"><span data-stu-id="a625b-108">Properties</span></span>
|<span data-ttu-id="a625b-109">Propriedade</span><span class="sxs-lookup"><span data-stu-id="a625b-109">Property</span></span>|<span data-ttu-id="a625b-110">Tipo</span><span class="sxs-lookup"><span data-stu-id="a625b-110">Type</span></span>|<span data-ttu-id="a625b-111">Descrição</span><span class="sxs-lookup"><span data-stu-id="a625b-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="a625b-112">ipAddressOrFQDN</span><span class="sxs-lookup"><span data-stu-id="a625b-112">ipAddressOrFQDN</span></span>|<span data-ttu-id="a625b-113">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="a625b-113">String</span></span>|<span data-ttu-id="a625b-114">O endereço IP ou o nome de domínio totalmente qualificado (FQDN).</span><span class="sxs-lookup"><span data-stu-id="a625b-114">The IP address or fully qualified domain name (FQDN).</span></span>|
|<span data-ttu-id="a625b-115">proxy</span><span class="sxs-lookup"><span data-stu-id="a625b-115">proxy</span></span>|<span data-ttu-id="a625b-116">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="a625b-116">String</span></span>|<span data-ttu-id="a625b-117">Endereço do proxy IP ou FQDN.</span><span class="sxs-lookup"><span data-stu-id="a625b-117">Proxy IP address or FQDN.</span></span>|

## <a name="relationships"></a><span data-ttu-id="a625b-118">Relações</span><span class="sxs-lookup"><span data-stu-id="a625b-118">Relationships</span></span>
<span data-ttu-id="a625b-119">Nenhum</span><span class="sxs-lookup"><span data-stu-id="a625b-119">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="a625b-120">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="a625b-120">JSON Representation</span></span>
<span data-ttu-id="a625b-121">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="a625b-121">Here is a JSON representation of the resource.</span></span>
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



