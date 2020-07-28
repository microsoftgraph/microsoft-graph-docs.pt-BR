---
title: recurso educationSynchronizationOAuth1ConnectionSettings
description: Quando o OAuth1 é usado para se conectar ao provedor de dados, esse tipo de configuração de conexão deve ser usado para configurar o perfil.
localization_priority: Normal
author: mmast-msft
ms.prod: education
doc_type: resourcePageType
ms.openlocfilehash: 525809121b07616c6eb5077f1b12d5b736586065
ms.sourcegitcommit: 2856a818ef3be0d4cfcbc9253906603bcc3d6325
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/28/2020
ms.locfileid: "45434918"
---
# <a name="educationsynchronizationoauth1connectionsettings-resource"></a><span data-ttu-id="1bc1c-103">recurso educationSynchronizationOAuth1ConnectionSettings</span><span class="sxs-lookup"><span data-stu-id="1bc1c-103">educationSynchronizationOAuth1ConnectionSettings resource</span></span>

<span data-ttu-id="1bc1c-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="1bc1c-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="1bc1c-105">Quando o OAuth1 é usado para se conectar ao provedor de dados, esse tipo de configuração de conexão deve ser usado para configurar o perfil.</span><span class="sxs-lookup"><span data-stu-id="1bc1c-105">When OAuth1 is to be used to connect to the data provider, this connection settings type should be used to set up the profile.</span></span>

<span data-ttu-id="1bc1c-106">Derivado de [educationSynchronizationConnectionSettings].</span><span class="sxs-lookup"><span data-stu-id="1bc1c-106">Derived from [educationSynchronizationConnectionSettings].</span></span>

## <a name="properties"></a><span data-ttu-id="1bc1c-107">Propriedades</span><span class="sxs-lookup"><span data-stu-id="1bc1c-107">Properties</span></span>

| <span data-ttu-id="1bc1c-108">Propriedade</span><span class="sxs-lookup"><span data-stu-id="1bc1c-108">Property</span></span>     | <span data-ttu-id="1bc1c-109">Tipo</span><span class="sxs-lookup"><span data-stu-id="1bc1c-109">Type</span></span>   | <span data-ttu-id="1bc1c-110">Descrição</span><span class="sxs-lookup"><span data-stu-id="1bc1c-110">Description</span></span>                                                                                                                |
| :----------- | :----- | :------------------------------------------------------------------------------------------------------------------------- |
| <span data-ttu-id="1bc1c-111">clientId</span><span class="sxs-lookup"><span data-stu-id="1bc1c-111">clientId</span></span>     | <span data-ttu-id="1bc1c-112">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="1bc1c-112">String</span></span> | <span data-ttu-id="1bc1c-113">ID do cliente usada para se conectar ao provedor.</span><span class="sxs-lookup"><span data-stu-id="1bc1c-113">Client ID used to connect to the provider.</span></span> <span data-ttu-id="1bc1c-114">Herdado de [educationSynchronizationConnectionSettings].</span><span class="sxs-lookup"><span data-stu-id="1bc1c-114">Inherited from [educationSynchronizationConnectionSettings].</span></span>                    |
| <span data-ttu-id="1bc1c-115">clientSecret</span><span class="sxs-lookup"><span data-stu-id="1bc1c-115">clientSecret</span></span> | <span data-ttu-id="1bc1c-116">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="1bc1c-116">String</span></span> | <span data-ttu-id="1bc1c-117">Segredo do cliente para autenticar a conexão com o provedor.</span><span class="sxs-lookup"><span data-stu-id="1bc1c-117">Client secret to authenticate the connection to the provider.</span></span> <span data-ttu-id="1bc1c-118">Herdado de [educationSynchronizationConnectionSettings].</span><span class="sxs-lookup"><span data-stu-id="1bc1c-118">Inherited from [educationSynchronizationConnectionSettings].</span></span> |

[educationsynchronizationconnectionsettings]: educationsynchronizationconnectionsettings.md

## <a name="json-representation"></a><span data-ttu-id="1bc1c-120">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="1bc1c-120">JSON representation</span></span>

<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.educationSynchronizationOAuth1ConnectionSettings"
}-->

```json
{
  "@odata.type": "microsoft.graph.educationSynchronizationOAuth1ConnectionSettings",
  "clientId": "String",
  "clientSecret": "String"
}
```
