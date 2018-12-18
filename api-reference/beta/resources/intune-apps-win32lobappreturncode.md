---
title: tipo de recurso de win32LobAppReturnCode
description: Contém propriedades de código de retorno para um aplicativo de Win32
author: tfitzmac
ms.openlocfilehash: 1ac6b01240e25d1a0163148e61851d6e9405aa44
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 12/18/2018
ms.locfileid: "27346232"
---
# <a name="win32lobappreturncode-resource-type"></a><span data-ttu-id="04951-103">tipo de recurso de win32LobAppReturnCode</span><span class="sxs-lookup"><span data-stu-id="04951-103">win32LobAppReturnCode resource type</span></span>

> <span data-ttu-id="04951-104">**Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e estão sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="04951-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="04951-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="04951-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="04951-106">**Observação:** O uso das APIs do Microsoft Graph para configurar controles e políticas do Intune ainda exige que o serviço do Intune seja [corretamente licenciado](https://go.microsoft.com/fwlink/?linkid=839381) pelo cliente.</span><span class="sxs-lookup"><span data-stu-id="04951-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="04951-107">Contém propriedades de código de retorno para um aplicativo de Win32</span><span class="sxs-lookup"><span data-stu-id="04951-107">Contains return code properties for a Win32 App</span></span>
## <a name="properties"></a><span data-ttu-id="04951-108">Propriedades</span><span class="sxs-lookup"><span data-stu-id="04951-108">Properties</span></span>
|<span data-ttu-id="04951-109">Propriedade</span><span class="sxs-lookup"><span data-stu-id="04951-109">Property</span></span>|<span data-ttu-id="04951-110">Tipo</span><span class="sxs-lookup"><span data-stu-id="04951-110">Type</span></span>|<span data-ttu-id="04951-111">Descrição</span><span class="sxs-lookup"><span data-stu-id="04951-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="04951-112">returnCode</span><span class="sxs-lookup"><span data-stu-id="04951-112">returnCode</span></span>|<span data-ttu-id="04951-113">Int32</span><span class="sxs-lookup"><span data-stu-id="04951-113">Int32</span></span>|<span data-ttu-id="04951-114">Código de retorno.</span><span class="sxs-lookup"><span data-stu-id="04951-114">Return code.</span></span>|
|<span data-ttu-id="04951-115">type</span><span class="sxs-lookup"><span data-stu-id="04951-115">type</span></span>|[<span data-ttu-id="04951-116">win32LobAppReturnCodeType</span><span class="sxs-lookup"><span data-stu-id="04951-116">win32LobAppReturnCodeType</span></span>](../resources/intune-apps-win32lobappreturncodetype.md)|<span data-ttu-id="04951-117">O tipo de código de retorno.</span><span class="sxs-lookup"><span data-stu-id="04951-117">The type of return code.</span></span> <span data-ttu-id="04951-118">Os valores possíveis são: `failed`, `success`, `softReboot`, `hardReboot`, `retry`.</span><span class="sxs-lookup"><span data-stu-id="04951-118">Possible values are: `failed`, `success`, `softReboot`, `hardReboot`, `retry`.</span></span>|

## <a name="relationships"></a><span data-ttu-id="04951-119">Relações</span><span class="sxs-lookup"><span data-stu-id="04951-119">Relationships</span></span>
<span data-ttu-id="04951-120">Nenhum</span><span class="sxs-lookup"><span data-stu-id="04951-120">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="04951-121">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="04951-121">JSON Representation</span></span>
<span data-ttu-id="04951-122">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="04951-122">Here is a JSON representation of the resource.</span></span>
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





