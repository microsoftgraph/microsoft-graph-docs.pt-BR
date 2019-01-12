---
title: tipo de recurso de win32LobAppInstallExperience
description: Contém propriedades de experiência de instalação para um aplicativo de Win32
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: 9eeadf7bc97f53278ef59fe06795bc7120d5bc2c
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/12/2019
ms.locfileid: "27986296"
---
# <a name="win32lobappinstallexperience-resource-type"></a><span data-ttu-id="6a7ad-103">tipo de recurso de win32LobAppInstallExperience</span><span class="sxs-lookup"><span data-stu-id="6a7ad-103">win32LobAppInstallExperience resource type</span></span>

> <span data-ttu-id="6a7ad-104">**Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e estão sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="6a7ad-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="6a7ad-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="6a7ad-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="6a7ad-106">**Observação:** O uso das APIs do Microsoft Graph para configurar controles e políticas do Intune ainda exige que o serviço do Intune seja [corretamente licenciado](https://go.microsoft.com/fwlink/?linkid=839381) pelo cliente.</span><span class="sxs-lookup"><span data-stu-id="6a7ad-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="6a7ad-107">Contém propriedades de experiência de instalação para um aplicativo de Win32</span><span class="sxs-lookup"><span data-stu-id="6a7ad-107">Contains installation experience properties for a Win32 App</span></span>
## <a name="properties"></a><span data-ttu-id="6a7ad-108">Propriedades</span><span class="sxs-lookup"><span data-stu-id="6a7ad-108">Properties</span></span>
|<span data-ttu-id="6a7ad-109">Propriedade</span><span class="sxs-lookup"><span data-stu-id="6a7ad-109">Property</span></span>|<span data-ttu-id="6a7ad-110">Tipo</span><span class="sxs-lookup"><span data-stu-id="6a7ad-110">Type</span></span>|<span data-ttu-id="6a7ad-111">Descrição</span><span class="sxs-lookup"><span data-stu-id="6a7ad-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="6a7ad-112">runAsAccount</span><span class="sxs-lookup"><span data-stu-id="6a7ad-112">runAsAccount</span></span>|[<span data-ttu-id="6a7ad-113">runAsAccountType</span><span class="sxs-lookup"><span data-stu-id="6a7ad-113">runAsAccountType</span></span>](../resources/intune-shared-runasaccounttype.md)|<span data-ttu-id="6a7ad-114">Indica o tipo de contexto de execução, em que o aplicativo é executado.</span><span class="sxs-lookup"><span data-stu-id="6a7ad-114">Indicates the type of execution context the app runs in.</span></span> <span data-ttu-id="6a7ad-115">Os valores possíveis são: `system`, `user`.</span><span class="sxs-lookup"><span data-stu-id="6a7ad-115">Possible values are: `system`, `user`.</span></span>|

## <a name="relationships"></a><span data-ttu-id="6a7ad-116">Relações</span><span class="sxs-lookup"><span data-stu-id="6a7ad-116">Relationships</span></span>
<span data-ttu-id="6a7ad-117">Nenhum</span><span class="sxs-lookup"><span data-stu-id="6a7ad-117">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="6a7ad-118">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="6a7ad-118">JSON Representation</span></span>
<span data-ttu-id="6a7ad-119">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="6a7ad-119">Here is a JSON representation of the resource.</span></span>
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





