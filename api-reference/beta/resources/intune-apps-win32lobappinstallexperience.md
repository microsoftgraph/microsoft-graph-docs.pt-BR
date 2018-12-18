---
title: tipo de recurso de win32LobAppInstallExperience
description: Contém propriedades de experiência de instalação para um aplicativo de Win32
author: tfitzmac
ms.openlocfilehash: c24ed0536416bd330fc2928a85cb0d5fce558256
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 12/18/2018
ms.locfileid: "27342158"
---
# <a name="win32lobappinstallexperience-resource-type"></a><span data-ttu-id="6bf52-103">tipo de recurso de win32LobAppInstallExperience</span><span class="sxs-lookup"><span data-stu-id="6bf52-103">win32LobAppInstallExperience resource type</span></span>

> <span data-ttu-id="6bf52-104">**Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e estão sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="6bf52-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="6bf52-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="6bf52-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="6bf52-106">**Observação:** O uso das APIs do Microsoft Graph para configurar controles e políticas do Intune ainda exige que o serviço do Intune seja [corretamente licenciado](https://go.microsoft.com/fwlink/?linkid=839381) pelo cliente.</span><span class="sxs-lookup"><span data-stu-id="6bf52-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="6bf52-107">Contém propriedades de experiência de instalação para um aplicativo de Win32</span><span class="sxs-lookup"><span data-stu-id="6bf52-107">Contains installation experience properties for a Win32 App</span></span>
## <a name="properties"></a><span data-ttu-id="6bf52-108">Propriedades</span><span class="sxs-lookup"><span data-stu-id="6bf52-108">Properties</span></span>
|<span data-ttu-id="6bf52-109">Propriedade</span><span class="sxs-lookup"><span data-stu-id="6bf52-109">Property</span></span>|<span data-ttu-id="6bf52-110">Tipo</span><span class="sxs-lookup"><span data-stu-id="6bf52-110">Type</span></span>|<span data-ttu-id="6bf52-111">Descrição</span><span class="sxs-lookup"><span data-stu-id="6bf52-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="6bf52-112">runAsAccount</span><span class="sxs-lookup"><span data-stu-id="6bf52-112">runAsAccount</span></span>|[<span data-ttu-id="6bf52-113">runAsAccountType</span><span class="sxs-lookup"><span data-stu-id="6bf52-113">runAsAccountType</span></span>](../resources/intune-shared-runasaccounttype.md)|<span data-ttu-id="6bf52-114">Indica o tipo de contexto de execução, em que o aplicativo é executado.</span><span class="sxs-lookup"><span data-stu-id="6bf52-114">Indicates the type of execution context the app runs in.</span></span> <span data-ttu-id="6bf52-115">Os valores possíveis são: `system`, `user`.</span><span class="sxs-lookup"><span data-stu-id="6bf52-115">Possible values are: `system`, `user`.</span></span>|

## <a name="relationships"></a><span data-ttu-id="6bf52-116">Relações</span><span class="sxs-lookup"><span data-stu-id="6bf52-116">Relationships</span></span>
<span data-ttu-id="6bf52-117">Nenhum</span><span class="sxs-lookup"><span data-stu-id="6bf52-117">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="6bf52-118">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="6bf52-118">JSON Representation</span></span>
<span data-ttu-id="6bf52-119">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="6bf52-119">Here is a JSON representation of the resource.</span></span>
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





