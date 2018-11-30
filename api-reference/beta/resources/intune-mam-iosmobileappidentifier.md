---
title: Tipo de recurso iosMobileAppIdentifier
description: O identificador de um aplicativo iOS.
ms.openlocfilehash: d95a9820c06d4d8e4122c3555e6e225c3d747761
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/29/2018
ms.locfileid: "27035246"
---
# <a name="iosmobileappidentifier-resource-type"></a><span data-ttu-id="ea93c-103">Tipo de recurso iosMobileAppIdentifier</span><span class="sxs-lookup"><span data-stu-id="ea93c-103">iosMobileAppIdentifier resource type</span></span>

> <span data-ttu-id="ea93c-104">**Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e estão sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="ea93c-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="ea93c-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="ea93c-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="ea93c-106">**Observação:** O uso das APIs do Microsoft Graph para configurar controles e políticas do Intune ainda exige que o serviço do Intune seja [corretamente licenciado](https://go.microsoft.com/fwlink/?linkid=839381) pelo cliente.</span><span class="sxs-lookup"><span data-stu-id="ea93c-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="ea93c-107">O identificador de um aplicativo iOS.</span><span class="sxs-lookup"><span data-stu-id="ea93c-107">The identifier for an iOS app.</span></span>

<span data-ttu-id="ea93c-108">Herda de [mobileAppIdentifier](../resources/intune-mam-mobileappidentifier.md)</span><span class="sxs-lookup"><span data-stu-id="ea93c-108">Inherits from [mobileAppIdentifier](../resources/intune-mam-mobileappidentifier.md)</span></span>

## <a name="properties"></a><span data-ttu-id="ea93c-109">Propriedades</span><span class="sxs-lookup"><span data-stu-id="ea93c-109">Properties</span></span>
|<span data-ttu-id="ea93c-110">Propriedade</span><span class="sxs-lookup"><span data-stu-id="ea93c-110">Property</span></span>|<span data-ttu-id="ea93c-111">Tipo</span><span class="sxs-lookup"><span data-stu-id="ea93c-111">Type</span></span>|<span data-ttu-id="ea93c-112">Descrição</span><span class="sxs-lookup"><span data-stu-id="ea93c-112">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="ea93c-113">bundleId</span><span class="sxs-lookup"><span data-stu-id="ea93c-113">bundleId</span></span>|<span data-ttu-id="ea93c-114">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="ea93c-114">String</span></span>|<span data-ttu-id="ea93c-115">O identificador de um aplicativo, conforme especificado na App Store.</span><span class="sxs-lookup"><span data-stu-id="ea93c-115">The identifier for an app, as specified in the app store.</span></span>|

## <a name="relationships"></a><span data-ttu-id="ea93c-116">Relações</span><span class="sxs-lookup"><span data-stu-id="ea93c-116">Relationships</span></span>
<span data-ttu-id="ea93c-117">Nenhum</span><span class="sxs-lookup"><span data-stu-id="ea93c-117">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="ea93c-118">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="ea93c-118">JSON Representation</span></span>
<span data-ttu-id="ea93c-119">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="ea93c-119">Here is a JSON representation of the resource.</span></span>
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





