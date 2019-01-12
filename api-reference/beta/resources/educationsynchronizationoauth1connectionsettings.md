---
title: recurso de educationSynchronizationOAuth1ConnectionSettings
description: Quando OAuth1 deve ser usado para se conectar ao provedor de dados, esse tipo de configurações de conexão deve ser usado para configurar o perfil.
localization_priority: Normal
author: mmast-msft
ms.prod: education
ms.openlocfilehash: 80921488e1a5e0dd3e4ab4e21b2ea08e05ad9cee
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/12/2019
ms.locfileid: "27990261"
---
# <a name="educationsynchronizationoauth1connectionsettings-resource"></a><span data-ttu-id="07757-103">recurso de educationSynchronizationOAuth1ConnectionSettings</span><span class="sxs-lookup"><span data-stu-id="07757-103">educationSynchronizationOAuth1ConnectionSettings resource</span></span>

> <span data-ttu-id="07757-104">**Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="07757-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="07757-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="07757-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="07757-106">Quando OAuth1 deve ser usado para se conectar ao provedor de dados, esse tipo de configurações de conexão deve ser usado para configurar o perfil.</span><span class="sxs-lookup"><span data-stu-id="07757-106">When OAuth1 is to be used to connect to the data provider, this connection settings type should be used to set up the profile.</span></span>

<span data-ttu-id="07757-107">Derivado do [educationSynchronizationConnectionSettings](educationsynchronizationconnectionsettings.md).</span><span class="sxs-lookup"><span data-stu-id="07757-107">Derived from [educationSynchronizationConnectionSettings](educationsynchronizationconnectionsettings.md).</span></span>

## <a name="properties"></a><span data-ttu-id="07757-108">Propriedades</span><span class="sxs-lookup"><span data-stu-id="07757-108">Properties</span></span>

<span data-ttu-id="07757-109">Não há propriedades adicionais são expostas por esse tipo.</span><span class="sxs-lookup"><span data-stu-id="07757-109">No additional properties are exposed by this type.</span></span>

## <a name="json-representation"></a><span data-ttu-id="07757-110">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="07757-110">JSON representation</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "#microsoft.graph.educationSynchronizationOAuth1ConnectionSettings"
}-->

```json
"connectionSettings": {
    "@odata.type": "#microsoft.graph.educationSynchronizationOAuth1ConnectionSettings",
    "clientId": "String",
    "clientSecret": "String"
}
```
