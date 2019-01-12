---
title: tipo de recurso de win32LobAppReturnCode
description: Contém propriedades de código de retorno para um aplicativo de Win32
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: 0728ee3c029331b37369172373ef1400dde37991
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/12/2019
ms.locfileid: "27927860"
---
# <a name="win32lobappreturncode-resource-type"></a><span data-ttu-id="f0403-103">tipo de recurso de win32LobAppReturnCode</span><span class="sxs-lookup"><span data-stu-id="f0403-103">win32LobAppReturnCode resource type</span></span>

> <span data-ttu-id="f0403-104">**Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e estão sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="f0403-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="f0403-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="f0403-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="f0403-106">**Observação:** O uso das APIs do Microsoft Graph para configurar controles e políticas do Intune ainda exige que o serviço do Intune seja [corretamente licenciado](https://go.microsoft.com/fwlink/?linkid=839381) pelo cliente.</span><span class="sxs-lookup"><span data-stu-id="f0403-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="f0403-107">Contém propriedades de código de retorno para um aplicativo de Win32</span><span class="sxs-lookup"><span data-stu-id="f0403-107">Contains return code properties for a Win32 App</span></span>
## <a name="properties"></a><span data-ttu-id="f0403-108">Propriedades</span><span class="sxs-lookup"><span data-stu-id="f0403-108">Properties</span></span>
|<span data-ttu-id="f0403-109">Propriedade</span><span class="sxs-lookup"><span data-stu-id="f0403-109">Property</span></span>|<span data-ttu-id="f0403-110">Tipo</span><span class="sxs-lookup"><span data-stu-id="f0403-110">Type</span></span>|<span data-ttu-id="f0403-111">Descrição</span><span class="sxs-lookup"><span data-stu-id="f0403-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="f0403-112">returnCode</span><span class="sxs-lookup"><span data-stu-id="f0403-112">returnCode</span></span>|<span data-ttu-id="f0403-113">Int32</span><span class="sxs-lookup"><span data-stu-id="f0403-113">Int32</span></span>|<span data-ttu-id="f0403-114">Código de retorno.</span><span class="sxs-lookup"><span data-stu-id="f0403-114">Return code.</span></span>|
|<span data-ttu-id="f0403-115">type</span><span class="sxs-lookup"><span data-stu-id="f0403-115">type</span></span>|[<span data-ttu-id="f0403-116">win32LobAppReturnCodeType</span><span class="sxs-lookup"><span data-stu-id="f0403-116">win32LobAppReturnCodeType</span></span>](../resources/intune-apps-win32lobappreturncodetype.md)|<span data-ttu-id="f0403-117">O tipo de código de retorno.</span><span class="sxs-lookup"><span data-stu-id="f0403-117">The type of return code.</span></span> <span data-ttu-id="f0403-118">Os valores possíveis são: `failed`, `success`, `softReboot`, `hardReboot`, `retry`.</span><span class="sxs-lookup"><span data-stu-id="f0403-118">Possible values are: `failed`, `success`, `softReboot`, `hardReboot`, `retry`.</span></span>|

## <a name="relationships"></a><span data-ttu-id="f0403-119">Relações</span><span class="sxs-lookup"><span data-stu-id="f0403-119">Relationships</span></span>
<span data-ttu-id="f0403-120">Nenhum</span><span class="sxs-lookup"><span data-stu-id="f0403-120">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="f0403-121">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="f0403-121">JSON Representation</span></span>
<span data-ttu-id="f0403-122">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="f0403-122">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.win32LobAppReturnCode"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.win32LobAppReturnCode",
  "returnCode": 1024,
  "type": "String"
}
```





