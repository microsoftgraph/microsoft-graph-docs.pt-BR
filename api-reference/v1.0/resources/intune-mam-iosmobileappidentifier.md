---
title: Tipo de recurso iosMobileAppIdentifier
description: O identificador de um aplicativo iOS.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 4b1dbebd30fecd15a916eef554bbdffd27b435f3
ms.sourcegitcommit: 13f474d3e71d32a5dfe2efebb351e3a1a5aa9685
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/04/2021
ms.locfileid: "52754522"
---
# <a name="iosmobileappidentifier-resource-type"></a><span data-ttu-id="753a2-103">Tipo de recurso iosMobileAppIdentifier</span><span class="sxs-lookup"><span data-stu-id="753a2-103">iosMobileAppIdentifier resource type</span></span>

<span data-ttu-id="753a2-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="753a2-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="753a2-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="753a2-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="753a2-106">O identificador de um aplicativo iOS.</span><span class="sxs-lookup"><span data-stu-id="753a2-106">The identifier for an iOS app.</span></span>


<span data-ttu-id="753a2-107">Herda de [mobileAppIdentifier](../resources/intune-mam-mobileappidentifier.md)</span><span class="sxs-lookup"><span data-stu-id="753a2-107">Inherits from [mobileAppIdentifier](../resources/intune-mam-mobileappidentifier.md)</span></span>

## <a name="properties"></a><span data-ttu-id="753a2-108">Propriedades</span><span class="sxs-lookup"><span data-stu-id="753a2-108">Properties</span></span>
|<span data-ttu-id="753a2-109">Propriedade</span><span class="sxs-lookup"><span data-stu-id="753a2-109">Property</span></span>|<span data-ttu-id="753a2-110">Tipo</span><span class="sxs-lookup"><span data-stu-id="753a2-110">Type</span></span>|<span data-ttu-id="753a2-111">Descrição</span><span class="sxs-lookup"><span data-stu-id="753a2-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="753a2-112">bundleId</span><span class="sxs-lookup"><span data-stu-id="753a2-112">bundleId</span></span>|<span data-ttu-id="753a2-113">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="753a2-113">String</span></span>|<span data-ttu-id="753a2-114">O identificador de um aplicativo, conforme especificado na App Store.</span><span class="sxs-lookup"><span data-stu-id="753a2-114">The identifier for an app, as specified in the app store.</span></span>|

## <a name="relationships"></a><span data-ttu-id="753a2-115">Relações</span><span class="sxs-lookup"><span data-stu-id="753a2-115">Relationships</span></span>
<span data-ttu-id="753a2-116">Nenhuma</span><span class="sxs-lookup"><span data-stu-id="753a2-116">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="753a2-117">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="753a2-117">JSON Representation</span></span>
<span data-ttu-id="753a2-118">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="753a2-118">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.iosMobileAppIdentifier"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.iosMobileAppIdentifier",
  "bundleId": "String"
}
```




