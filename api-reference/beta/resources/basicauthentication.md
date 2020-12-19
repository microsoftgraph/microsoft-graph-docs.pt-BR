---
title: tipo de recurso basicAuthentication
description: Representa a configuração para usar a autenticação básica em uma chamada de API.
author: nickgmicrosoft
localization_priority: Normal
ms.prod: microsoft-identity-platform
doc_type: resourcePageType
ms.openlocfilehash: 9de5fad9746e8562f51d1ddc8fcea350c41979ed
ms.sourcegitcommit: 424735f8ab46de76b9d850e10c7d97ffd164f62a
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 12/19/2020
ms.locfileid: "49720090"
---
# <a name="basicauthentication-resource-type"></a><span data-ttu-id="57609-103">tipo de recurso basicAuthentication</span><span class="sxs-lookup"><span data-stu-id="57609-103">basicAuthentication resource type</span></span>

<span data-ttu-id="57609-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="57609-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="57609-105">Representa a configuração para usar a autenticação básica HTTP, que envolve um nome de usuário e senha em uma chamada de API.</span><span class="sxs-lookup"><span data-stu-id="57609-105">Represents configuration for using HTTP Basic authentication, which entails a username and password, in an API call.</span></span> <span data-ttu-id="57609-106">O nome de usuário e a senha são enviados como o cabeçalho de autorização, como a `Basic {value}` `value` versão base 64 codificada de nome de usuário: senha.</span><span class="sxs-lookup"><span data-stu-id="57609-106">The username and password is sent as the Authorization header as `Basic {value}` where `value` is base 64 encoded version of username:password.</span></span>

<span data-ttu-id="57609-107">Herda de [apiAuthenticationConfigurationBase](../resources/apiauthenticationconfigurationbase.md).</span><span class="sxs-lookup"><span data-stu-id="57609-107">Inherits from [apiAuthenticationConfigurationBase](../resources/apiauthenticationconfigurationbase.md).</span></span>

## <a name="properties"></a><span data-ttu-id="57609-108">Propriedades</span><span class="sxs-lookup"><span data-stu-id="57609-108">Properties</span></span>

|<span data-ttu-id="57609-109">Propriedade</span><span class="sxs-lookup"><span data-stu-id="57609-109">Property</span></span>|<span data-ttu-id="57609-110">Tipo</span><span class="sxs-lookup"><span data-stu-id="57609-110">Type</span></span>|<span data-ttu-id="57609-111">Descrição</span><span class="sxs-lookup"><span data-stu-id="57609-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="57609-112">username</span><span class="sxs-lookup"><span data-stu-id="57609-112">username</span></span>|<span data-ttu-id="57609-113">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="57609-113">String</span></span>| <span data-ttu-id="57609-114">O nome de usuário.</span><span class="sxs-lookup"><span data-stu-id="57609-114">The username.</span></span> |
|<span data-ttu-id="57609-115">password</span><span class="sxs-lookup"><span data-stu-id="57609-115">password</span></span>|<span data-ttu-id="57609-116">String</span><span class="sxs-lookup"><span data-stu-id="57609-116">String</span></span>| <span data-ttu-id="57609-117">A senha.</span><span class="sxs-lookup"><span data-stu-id="57609-117">The password.</span></span> <span data-ttu-id="57609-118">Ele não é retornado nas respostas.</span><span class="sxs-lookup"><span data-stu-id="57609-118">It is not returned in the responses.</span></span> |

## <a name="relationships"></a><span data-ttu-id="57609-119">Relações</span><span class="sxs-lookup"><span data-stu-id="57609-119">Relationships</span></span>

<span data-ttu-id="57609-120">Nenhum</span><span class="sxs-lookup"><span data-stu-id="57609-120">None.</span></span>

## <a name="json-representation"></a><span data-ttu-id="57609-121">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="57609-121">JSON representation</span></span>

<span data-ttu-id="57609-122">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="57609-122">The following is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.basicAuthentication"
}
-->

``` json
{
  "@odata.type": "#microsoft.graph.basicAuthentication",
  "password": "String",
  "username": "String"
}
```
