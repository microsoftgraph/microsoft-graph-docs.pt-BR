---
title: tipo de recurso androidDeviceOwnerGlobalProxyAutoConfig
description: Configuração automática de proxy global de proprietário do dispositivo Android.
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: e15b3009537bd55eb7d4af6d93bbea3b53f3325a
ms.sourcegitcommit: 0dcabe677927c259c2ddcefd0d5e2a2aef065e8b
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 10/16/2019
ms.locfileid: "37538648"
---
# <a name="androiddeviceownerglobalproxyautoconfig-resource-type"></a><span data-ttu-id="324b9-103">tipo de recurso androidDeviceOwnerGlobalProxyAutoConfig</span><span class="sxs-lookup"><span data-stu-id="324b9-103">androidDeviceOwnerGlobalProxyAutoConfig resource type</span></span>

> <span data-ttu-id="324b9-104">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="324b9-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="324b9-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="324b9-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="324b9-106">Configuração automática de proxy global de proprietário do dispositivo Android.</span><span class="sxs-lookup"><span data-stu-id="324b9-106">Android Device Owner Global Proxy Auto Config.</span></span>


<span data-ttu-id="324b9-107">Herda de [androidDeviceOwnerGlobalProxy](../resources/intune-deviceconfig-androiddeviceownerglobalproxy.md)</span><span class="sxs-lookup"><span data-stu-id="324b9-107">Inherits from [androidDeviceOwnerGlobalProxy](../resources/intune-deviceconfig-androiddeviceownerglobalproxy.md)</span></span>

## <a name="properties"></a><span data-ttu-id="324b9-108">Propriedades</span><span class="sxs-lookup"><span data-stu-id="324b9-108">Properties</span></span>
|<span data-ttu-id="324b9-109">Propriedade</span><span class="sxs-lookup"><span data-stu-id="324b9-109">Property</span></span>|<span data-ttu-id="324b9-110">Tipo</span><span class="sxs-lookup"><span data-stu-id="324b9-110">Type</span></span>|<span data-ttu-id="324b9-111">Descrição</span><span class="sxs-lookup"><span data-stu-id="324b9-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="324b9-112">proxyAutoConfigURL</span><span class="sxs-lookup"><span data-stu-id="324b9-112">proxyAutoConfigURL</span></span>|<span data-ttu-id="324b9-113">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="324b9-113">String</span></span>|<span data-ttu-id="324b9-114">A URL de configuração automática do proxy</span><span class="sxs-lookup"><span data-stu-id="324b9-114">The proxy auto-config URL</span></span>|

## <a name="relationships"></a><span data-ttu-id="324b9-115">Relações</span><span class="sxs-lookup"><span data-stu-id="324b9-115">Relationships</span></span>
<span data-ttu-id="324b9-116">Nenhum</span><span class="sxs-lookup"><span data-stu-id="324b9-116">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="324b9-117">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="324b9-117">JSON Representation</span></span>
<span data-ttu-id="324b9-118">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="324b9-118">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.androidDeviceOwnerGlobalProxyAutoConfig"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.androidDeviceOwnerGlobalProxyAutoConfig",
  "proxyAutoConfigURL": "String"
}
```



