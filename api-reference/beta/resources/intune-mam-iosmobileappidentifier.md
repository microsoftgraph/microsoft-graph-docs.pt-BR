---
title: Tipo de recurso iosMobileAppIdentifier
description: O identificador de um aplicativo iOS.
author: tfitzmac
localization_priority: Normal
ms.openlocfilehash: a5540ba03dffe0dcedbfe3e59c6b004434bb0ed4
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/11/2019
ms.locfileid: "27828354"
---
# <a name="iosmobileappidentifier-resource-type"></a><span data-ttu-id="ed413-103">Tipo de recurso iosMobileAppIdentifier</span><span class="sxs-lookup"><span data-stu-id="ed413-103">iosMobileAppIdentifier resource type</span></span>

> <span data-ttu-id="ed413-104">**Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e estão sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="ed413-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="ed413-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="ed413-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="ed413-106">**Observação:** O uso das APIs do Microsoft Graph para configurar controles e políticas do Intune ainda exige que o serviço do Intune seja [corretamente licenciado](https://go.microsoft.com/fwlink/?linkid=839381) pelo cliente.</span><span class="sxs-lookup"><span data-stu-id="ed413-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="ed413-107">O identificador de um aplicativo iOS.</span><span class="sxs-lookup"><span data-stu-id="ed413-107">The identifier for an iOS app.</span></span>

<span data-ttu-id="ed413-108">Herda de [mobileAppIdentifier](../resources/intune-mam-mobileappidentifier.md)</span><span class="sxs-lookup"><span data-stu-id="ed413-108">Inherits from [mobileAppIdentifier](../resources/intune-mam-mobileappidentifier.md)</span></span>

## <a name="properties"></a><span data-ttu-id="ed413-109">Propriedades</span><span class="sxs-lookup"><span data-stu-id="ed413-109">Properties</span></span>
|<span data-ttu-id="ed413-110">Propriedade</span><span class="sxs-lookup"><span data-stu-id="ed413-110">Property</span></span>|<span data-ttu-id="ed413-111">Tipo</span><span class="sxs-lookup"><span data-stu-id="ed413-111">Type</span></span>|<span data-ttu-id="ed413-112">Descrição</span><span class="sxs-lookup"><span data-stu-id="ed413-112">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="ed413-113">bundleId</span><span class="sxs-lookup"><span data-stu-id="ed413-113">bundleId</span></span>|<span data-ttu-id="ed413-114">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="ed413-114">String</span></span>|<span data-ttu-id="ed413-115">O identificador de um aplicativo, conforme especificado na App Store.</span><span class="sxs-lookup"><span data-stu-id="ed413-115">The identifier for an app, as specified in the app store.</span></span>|

## <a name="relationships"></a><span data-ttu-id="ed413-116">Relações</span><span class="sxs-lookup"><span data-stu-id="ed413-116">Relationships</span></span>
<span data-ttu-id="ed413-117">Nenhum</span><span class="sxs-lookup"><span data-stu-id="ed413-117">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="ed413-118">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="ed413-118">JSON Representation</span></span>
<span data-ttu-id="ed413-119">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="ed413-119">Here is a JSON representation of the resource.</span></span>
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





