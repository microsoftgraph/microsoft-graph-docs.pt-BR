---
title: Tipo de recurso iosMobileAppIdentifier
description: O identificador de um aplicativo iOS.
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: ddd09f6d1f0d49b00282c55bfa6dcbef1fcb1d2c
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/23/2019
ms.locfileid: "29409927"
---
# <a name="iosmobileappidentifier-resource-type"></a><span data-ttu-id="af2b6-103">Tipo de recurso iosMobileAppIdentifier</span><span class="sxs-lookup"><span data-stu-id="af2b6-103">iosMobileAppIdentifier resource type</span></span>

> <span data-ttu-id="af2b6-104">**Importante:** APIs sob a versão /beta no Microsoft Graph estão sujeitos a alterações.</span><span class="sxs-lookup"><span data-stu-id="af2b6-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="af2b6-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="af2b6-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="af2b6-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença de Intune ativa](https://go.microsoft.com/fwlink/?linkid=839381) para o inquilino.</span><span class="sxs-lookup"><span data-stu-id="af2b6-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="af2b6-107">O identificador de um aplicativo iOS.</span><span class="sxs-lookup"><span data-stu-id="af2b6-107">The identifier for an iOS app.</span></span>


<span data-ttu-id="af2b6-108">Herda de [mobileAppIdentifier](../resources/intune-mam-mobileappidentifier.md)</span><span class="sxs-lookup"><span data-stu-id="af2b6-108">Inherits from [mobileAppIdentifier](../resources/intune-mam-mobileappidentifier.md)</span></span>

## <a name="properties"></a><span data-ttu-id="af2b6-109">Propriedades</span><span class="sxs-lookup"><span data-stu-id="af2b6-109">Properties</span></span>
|<span data-ttu-id="af2b6-110">Propriedade</span><span class="sxs-lookup"><span data-stu-id="af2b6-110">Property</span></span>|<span data-ttu-id="af2b6-111">Tipo</span><span class="sxs-lookup"><span data-stu-id="af2b6-111">Type</span></span>|<span data-ttu-id="af2b6-112">Descrição</span><span class="sxs-lookup"><span data-stu-id="af2b6-112">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="af2b6-113">bundleId</span><span class="sxs-lookup"><span data-stu-id="af2b6-113">bundleId</span></span>|<span data-ttu-id="af2b6-114">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="af2b6-114">String</span></span>|<span data-ttu-id="af2b6-115">O identificador de um aplicativo, conforme especificado na App Store.</span><span class="sxs-lookup"><span data-stu-id="af2b6-115">The identifier for an app, as specified in the app store.</span></span>|

## <a name="relationships"></a><span data-ttu-id="af2b6-116">Relações</span><span class="sxs-lookup"><span data-stu-id="af2b6-116">Relationships</span></span>
<span data-ttu-id="af2b6-117">Nenhum</span><span class="sxs-lookup"><span data-stu-id="af2b6-117">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="af2b6-118">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="af2b6-118">JSON Representation</span></span>
<span data-ttu-id="af2b6-119">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="af2b6-119">Here is a JSON representation of the resource.</span></span>
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




