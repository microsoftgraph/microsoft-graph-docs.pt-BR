---
title: tipo de recurso de win32LobAppInstallExperience
description: Contém propriedades de experiência de instalação para um aplicativo de Win32
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: 240000dfceaa2ef4e973167cbd3b5a743d346892
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/23/2019
ms.locfileid: "29406686"
---
# <a name="win32lobappinstallexperience-resource-type"></a><span data-ttu-id="94b99-103">tipo de recurso de win32LobAppInstallExperience</span><span class="sxs-lookup"><span data-stu-id="94b99-103">win32LobAppInstallExperience resource type</span></span>

> <span data-ttu-id="94b99-104">**Importante:** APIs sob a versão /beta no Microsoft Graph estão sujeitos a alterações.</span><span class="sxs-lookup"><span data-stu-id="94b99-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="94b99-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="94b99-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="94b99-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença de Intune ativa](https://go.microsoft.com/fwlink/?linkid=839381) para o inquilino.</span><span class="sxs-lookup"><span data-stu-id="94b99-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="94b99-107">Contém propriedades de experiência de instalação para um aplicativo de Win32</span><span class="sxs-lookup"><span data-stu-id="94b99-107">Contains installation experience properties for a Win32 App</span></span>

## <a name="properties"></a><span data-ttu-id="94b99-108">Propriedades</span><span class="sxs-lookup"><span data-stu-id="94b99-108">Properties</span></span>
|<span data-ttu-id="94b99-109">Propriedade</span><span class="sxs-lookup"><span data-stu-id="94b99-109">Property</span></span>|<span data-ttu-id="94b99-110">Tipo</span><span class="sxs-lookup"><span data-stu-id="94b99-110">Type</span></span>|<span data-ttu-id="94b99-111">Descrição</span><span class="sxs-lookup"><span data-stu-id="94b99-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="94b99-112">runAsAccount</span><span class="sxs-lookup"><span data-stu-id="94b99-112">runAsAccount</span></span>|[<span data-ttu-id="94b99-113">runAsAccountType</span><span class="sxs-lookup"><span data-stu-id="94b99-113">runAsAccountType</span></span>](../resources/intune-shared-runasaccounttype.md)|<span data-ttu-id="94b99-114">Indica o tipo de contexto de execução, em que o aplicativo é executado.</span><span class="sxs-lookup"><span data-stu-id="94b99-114">Indicates the type of execution context the app runs in.</span></span> <span data-ttu-id="94b99-115">Os valores possíveis são: `system`, `user`.</span><span class="sxs-lookup"><span data-stu-id="94b99-115">Possible values are: `system`, `user`.</span></span>|

## <a name="relationships"></a><span data-ttu-id="94b99-116">Relações</span><span class="sxs-lookup"><span data-stu-id="94b99-116">Relationships</span></span>
<span data-ttu-id="94b99-117">Nenhum</span><span class="sxs-lookup"><span data-stu-id="94b99-117">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="94b99-118">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="94b99-118">JSON Representation</span></span>
<span data-ttu-id="94b99-119">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="94b99-119">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.win32LobAppInstallExperience"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.win32LobAppInstallExperience",
  "runAsAccount": "String"
}
```




