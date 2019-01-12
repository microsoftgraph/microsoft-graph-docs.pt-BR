---
title: Tipo de recurso iosMobileAppIdentifier
description: O identificador de um aplicativo iOS.
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: 134f6e27b6fb113516fd119211e245fd77b2ae75
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/12/2019
ms.locfileid: "27919523"
---
# <a name="iosmobileappidentifier-resource-type"></a><span data-ttu-id="21332-103">Tipo de recurso iosMobileAppIdentifier</span><span class="sxs-lookup"><span data-stu-id="21332-103">iosMobileAppIdentifier resource type</span></span>

> <span data-ttu-id="21332-104">**Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e estão sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="21332-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="21332-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="21332-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="21332-106">**Observação:** O uso das APIs do Microsoft Graph para configurar controles e políticas do Intune ainda exige que o serviço do Intune seja [corretamente licenciado](https://go.microsoft.com/fwlink/?linkid=839381) pelo cliente.</span><span class="sxs-lookup"><span data-stu-id="21332-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="21332-107">O identificador de um aplicativo iOS.</span><span class="sxs-lookup"><span data-stu-id="21332-107">The identifier for an iOS app.</span></span>

<span data-ttu-id="21332-108">Herda de [mobileAppIdentifier](../resources/intune-mam-mobileappidentifier.md)</span><span class="sxs-lookup"><span data-stu-id="21332-108">Inherits from [mobileAppIdentifier](../resources/intune-mam-mobileappidentifier.md)</span></span>

## <a name="properties"></a><span data-ttu-id="21332-109">Propriedades</span><span class="sxs-lookup"><span data-stu-id="21332-109">Properties</span></span>
|<span data-ttu-id="21332-110">Propriedade</span><span class="sxs-lookup"><span data-stu-id="21332-110">Property</span></span>|<span data-ttu-id="21332-111">Tipo</span><span class="sxs-lookup"><span data-stu-id="21332-111">Type</span></span>|<span data-ttu-id="21332-112">Descrição</span><span class="sxs-lookup"><span data-stu-id="21332-112">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="21332-113">bundleId</span><span class="sxs-lookup"><span data-stu-id="21332-113">bundleId</span></span>|<span data-ttu-id="21332-114">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="21332-114">String</span></span>|<span data-ttu-id="21332-115">O identificador de um aplicativo, conforme especificado na App Store.</span><span class="sxs-lookup"><span data-stu-id="21332-115">The identifier for an app, as specified in the app store.</span></span>|

## <a name="relationships"></a><span data-ttu-id="21332-116">Relações</span><span class="sxs-lookup"><span data-stu-id="21332-116">Relationships</span></span>
<span data-ttu-id="21332-117">Nenhum</span><span class="sxs-lookup"><span data-stu-id="21332-117">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="21332-118">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="21332-118">JSON Representation</span></span>
<span data-ttu-id="21332-119">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="21332-119">Here is a JSON representation of the resource.</span></span>
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





