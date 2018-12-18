---
title: Tipo de recurso iosHomeScreenItem
description: Representa um item na tela inicial do iOS
author: tfitzmac
ms.openlocfilehash: 6a8d71e01ca8f2c284bcc3eddd7eb39b87c025d7
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 12/18/2018
ms.locfileid: "27328186"
---
# <a name="ioshomescreenitem-resource-type"></a><span data-ttu-id="bf72a-103">Tipo de recurso iosHomeScreenItem</span><span class="sxs-lookup"><span data-stu-id="bf72a-103">iosHomeScreenItem resource type</span></span>

> <span data-ttu-id="bf72a-104">**Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e estão sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="bf72a-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="bf72a-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="bf72a-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="bf72a-106">**Observação:** O uso das APIs do Microsoft Graph para configurar controles e políticas do Intune ainda exige que o serviço do Intune seja [corretamente licenciado](https://go.microsoft.com/fwlink/?linkid=839381) pelo cliente.</span><span class="sxs-lookup"><span data-stu-id="bf72a-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="bf72a-107">Representa um item na tela inicial do iOS</span><span class="sxs-lookup"><span data-stu-id="bf72a-107">Represents an item on the iOS Home Screen</span></span>
## <a name="properties"></a><span data-ttu-id="bf72a-108">Propriedades</span><span class="sxs-lookup"><span data-stu-id="bf72a-108">Properties</span></span>
|<span data-ttu-id="bf72a-109">Propriedade</span><span class="sxs-lookup"><span data-stu-id="bf72a-109">Property</span></span>|<span data-ttu-id="bf72a-110">Tipo</span><span class="sxs-lookup"><span data-stu-id="bf72a-110">Type</span></span>|<span data-ttu-id="bf72a-111">Descrição</span><span class="sxs-lookup"><span data-stu-id="bf72a-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="bf72a-112">displayName</span><span class="sxs-lookup"><span data-stu-id="bf72a-112">displayName</span></span>|<span data-ttu-id="bf72a-113">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="bf72a-113">String</span></span>|<span data-ttu-id="bf72a-114">Nome do aplicativo</span><span class="sxs-lookup"><span data-stu-id="bf72a-114">Name of the app</span></span>|

## <a name="relationships"></a><span data-ttu-id="bf72a-115">Relações</span><span class="sxs-lookup"><span data-stu-id="bf72a-115">Relationships</span></span>
<span data-ttu-id="bf72a-116">Nenhum</span><span class="sxs-lookup"><span data-stu-id="bf72a-116">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="bf72a-117">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="bf72a-117">JSON Representation</span></span>
<span data-ttu-id="bf72a-118">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="bf72a-118">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.iosHomeScreenItem"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.iosHomeScreenItem",
  "displayName": "String"
}
```





