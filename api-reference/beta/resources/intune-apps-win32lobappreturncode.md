---
title: tipo de recurso de win32LobAppReturnCode
description: Contém propriedades de código de retorno para um aplicativo de Win32
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: e6357d0ac6aab87e236e02d60454d1b45aa98fe1
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/23/2019
ms.locfileid: "29404355"
---
# <a name="win32lobappreturncode-resource-type"></a><span data-ttu-id="af8b0-103">tipo de recurso de win32LobAppReturnCode</span><span class="sxs-lookup"><span data-stu-id="af8b0-103">win32LobAppReturnCode resource type</span></span>

> <span data-ttu-id="af8b0-104">**Importante:** APIs sob a versão /beta no Microsoft Graph estão sujeitos a alterações.</span><span class="sxs-lookup"><span data-stu-id="af8b0-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="af8b0-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="af8b0-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="af8b0-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença de Intune ativa](https://go.microsoft.com/fwlink/?linkid=839381) para o inquilino.</span><span class="sxs-lookup"><span data-stu-id="af8b0-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="af8b0-107">Contém propriedades de código de retorno para um aplicativo de Win32</span><span class="sxs-lookup"><span data-stu-id="af8b0-107">Contains return code properties for a Win32 App</span></span>

## <a name="properties"></a><span data-ttu-id="af8b0-108">Propriedades</span><span class="sxs-lookup"><span data-stu-id="af8b0-108">Properties</span></span>
|<span data-ttu-id="af8b0-109">Propriedade</span><span class="sxs-lookup"><span data-stu-id="af8b0-109">Property</span></span>|<span data-ttu-id="af8b0-110">Tipo</span><span class="sxs-lookup"><span data-stu-id="af8b0-110">Type</span></span>|<span data-ttu-id="af8b0-111">Descrição</span><span class="sxs-lookup"><span data-stu-id="af8b0-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="af8b0-112">returnCode</span><span class="sxs-lookup"><span data-stu-id="af8b0-112">returnCode</span></span>|<span data-ttu-id="af8b0-113">Int32</span><span class="sxs-lookup"><span data-stu-id="af8b0-113">Int32</span></span>|<span data-ttu-id="af8b0-114">Código de retorno.</span><span class="sxs-lookup"><span data-stu-id="af8b0-114">Return code.</span></span>|
|<span data-ttu-id="af8b0-115">type</span><span class="sxs-lookup"><span data-stu-id="af8b0-115">type</span></span>|[<span data-ttu-id="af8b0-116">win32LobAppReturnCodeType</span><span class="sxs-lookup"><span data-stu-id="af8b0-116">win32LobAppReturnCodeType</span></span>](../resources/intune-apps-win32lobappreturncodetype.md)|<span data-ttu-id="af8b0-117">O tipo de código de retorno.</span><span class="sxs-lookup"><span data-stu-id="af8b0-117">The type of return code.</span></span> <span data-ttu-id="af8b0-118">Os valores possíveis são: `failed`, `success`, `softReboot`, `hardReboot`, `retry`.</span><span class="sxs-lookup"><span data-stu-id="af8b0-118">Possible values are: `failed`, `success`, `softReboot`, `hardReboot`, `retry`.</span></span>|

## <a name="relationships"></a><span data-ttu-id="af8b0-119">Relações</span><span class="sxs-lookup"><span data-stu-id="af8b0-119">Relationships</span></span>
<span data-ttu-id="af8b0-120">Nenhum</span><span class="sxs-lookup"><span data-stu-id="af8b0-120">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="af8b0-121">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="af8b0-121">JSON Representation</span></span>
<span data-ttu-id="af8b0-122">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="af8b0-122">Here is a JSON representation of the resource.</span></span>
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




