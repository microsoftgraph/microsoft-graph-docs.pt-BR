---
title: Tipo de recurso edgeSearchEngineBase
description: Permite aos administradores de TI definir um mecanismo de pesquisa padrão para dispositivos controlados por MDM. Os usuários podem substituí-lo e alterar o mecanismo de pesquisa padrão fornecido, caso a política AllowSearchEngineCustomization não esteja definida.
author: tfitzmac
ms.openlocfilehash: c60dd1786f5a211947c02f1a9f5f048737ba3788
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 12/18/2018
ms.locfileid: "27346498"
---
# <a name="edgesearchenginebase-resource-type"></a><span data-ttu-id="85213-104">Tipo de recurso edgeSearchEngineBase</span><span class="sxs-lookup"><span data-stu-id="85213-104">edgeSearchEngineBase resource type</span></span>

> <span data-ttu-id="85213-105">**Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e estão sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="85213-105">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="85213-106">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="85213-106">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="85213-107">**Observação:** O uso das APIs do Microsoft Graph para configurar controles e políticas do Intune ainda exige que o serviço do Intune seja [corretamente licenciado](https://go.microsoft.com/fwlink/?linkid=839381) pelo cliente.</span><span class="sxs-lookup"><span data-stu-id="85213-107">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="85213-108">Permite aos administradores de TI definir um mecanismo de pesquisa padrão para dispositivos controlados por MDM.</span><span class="sxs-lookup"><span data-stu-id="85213-108">Allows IT admins to set a default search engine for MDM-Controlled devices.</span></span> <span data-ttu-id="85213-109">Os usuários podem substituí-lo e alterar o mecanismo de pesquisa padrão fornecido, caso a política AllowSearchEngineCustomization não esteja definida.</span><span class="sxs-lookup"><span data-stu-id="85213-109">Users can override this and change their default search engine provided the AllowSearchEngineCustomization policy is not set.</span></span>
## <a name="properties"></a><span data-ttu-id="85213-110">Propriedades</span><span class="sxs-lookup"><span data-stu-id="85213-110">Properties</span></span>
|<span data-ttu-id="85213-111">Propriedade</span><span class="sxs-lookup"><span data-stu-id="85213-111">Property</span></span>|<span data-ttu-id="85213-112">Tipo</span><span class="sxs-lookup"><span data-stu-id="85213-112">Type</span></span>|<span data-ttu-id="85213-113">Descrição</span><span class="sxs-lookup"><span data-stu-id="85213-113">Description</span></span>|
|:---|:---|:---|

## <a name="relationships"></a><span data-ttu-id="85213-114">Relações</span><span class="sxs-lookup"><span data-stu-id="85213-114">Relationships</span></span>
<span data-ttu-id="85213-115">Nenhum</span><span class="sxs-lookup"><span data-stu-id="85213-115">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="85213-116">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="85213-116">JSON Representation</span></span>
<span data-ttu-id="85213-117">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="85213-117">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.edgeSearchEngineBase"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.edgeSearchEngineBase"
}
```





