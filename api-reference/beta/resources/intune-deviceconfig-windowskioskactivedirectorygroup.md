---
title: tipo de recurso de windowsKioskActiveDirectoryGroup
description: A classe usada para identificar um grupo de diretório do Windows Azure para a configuração de quiosque
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: 632396b727448032f198a54b97ba0a46b961abe5
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/12/2019
ms.locfileid: "27955230"
---
# <a name="windowskioskactivedirectorygroup-resource-type"></a><span data-ttu-id="4c7f8-103">tipo de recurso de windowsKioskActiveDirectoryGroup</span><span class="sxs-lookup"><span data-stu-id="4c7f8-103">windowsKioskActiveDirectoryGroup resource type</span></span>

> <span data-ttu-id="4c7f8-104">**Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e estão sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="4c7f8-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="4c7f8-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="4c7f8-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="4c7f8-106">**Observação:** O uso das APIs do Microsoft Graph para configurar controles e políticas do Intune ainda exige que o serviço do Intune seja [corretamente licenciado](https://go.microsoft.com/fwlink/?linkid=839381) pelo cliente.</span><span class="sxs-lookup"><span data-stu-id="4c7f8-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="4c7f8-107">A classe usada para identificar um grupo de diretório do Windows Azure para a configuração de quiosque</span><span class="sxs-lookup"><span data-stu-id="4c7f8-107">The class used to identify an Azure Directory group for the kiosk configuration</span></span>

<span data-ttu-id="4c7f8-108">Herda de [windowsKioskUser](../resources/intune-deviceconfig-windowskioskuser.md)</span><span class="sxs-lookup"><span data-stu-id="4c7f8-108">Inherits from [windowsKioskUser](../resources/intune-deviceconfig-windowskioskuser.md)</span></span>

## <a name="properties"></a><span data-ttu-id="4c7f8-109">Propriedades</span><span class="sxs-lookup"><span data-stu-id="4c7f8-109">Properties</span></span>
|<span data-ttu-id="4c7f8-110">Propriedade</span><span class="sxs-lookup"><span data-stu-id="4c7f8-110">Property</span></span>|<span data-ttu-id="4c7f8-111">Tipo</span><span class="sxs-lookup"><span data-stu-id="4c7f8-111">Type</span></span>|<span data-ttu-id="4c7f8-112">Descrição</span><span class="sxs-lookup"><span data-stu-id="4c7f8-112">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="4c7f8-113">groupName</span><span class="sxs-lookup"><span data-stu-id="4c7f8-113">groupName</span></span>|<span data-ttu-id="4c7f8-114">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="4c7f8-114">String</span></span>|<span data-ttu-id="4c7f8-115">O nome do grupo AD que será bloqueado para esta configuração de quiosque</span><span class="sxs-lookup"><span data-stu-id="4c7f8-115">The name of the AD group that will be locked to this kiosk configuration</span></span>|

## <a name="relationships"></a><span data-ttu-id="4c7f8-116">Relações</span><span class="sxs-lookup"><span data-stu-id="4c7f8-116">Relationships</span></span>
<span data-ttu-id="4c7f8-117">Nenhum</span><span class="sxs-lookup"><span data-stu-id="4c7f8-117">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="4c7f8-118">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="4c7f8-118">JSON Representation</span></span>
<span data-ttu-id="4c7f8-119">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="4c7f8-119">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.windowsKioskActiveDirectoryGroup"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.windowsKioskActiveDirectoryGroup",
  "groupName": "String"
}
```





