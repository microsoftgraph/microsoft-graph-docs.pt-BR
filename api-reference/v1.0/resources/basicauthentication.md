---
title: Tipo de recurso basicAuthentication
description: Representa a configuração para o uso da autenticação básica em uma chamada de API.
author: nickgmicrosoft
localization_priority: Normal
ms.prod: identity-and-sign-in
doc_type: resourcePageType
ms.openlocfilehash: 9bb61e297a6a668631da654383e13ee1dbf8ef79
ms.sourcegitcommit: d033e7de12bccf92efcbe40c7b671e419a3e5b94
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/17/2021
ms.locfileid: "51882381"
---
# <a name="basicauthentication-resource-type"></a><span data-ttu-id="1e0fa-103">Tipo de recurso basicAuthentication</span><span class="sxs-lookup"><span data-stu-id="1e0fa-103">basicAuthentication resource type</span></span>

<span data-ttu-id="1e0fa-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="1e0fa-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="1e0fa-105">Representa a configuração para o uso da autenticação HTTP Basic, que envolve um nome de usuário e uma senha, em uma chamada de API.</span><span class="sxs-lookup"><span data-stu-id="1e0fa-105">Represents configuration for using HTTP Basic authentication, which entails a username and password, in an API call.</span></span> <span data-ttu-id="1e0fa-106">O nome de usuário e a senha são enviados como o header de Autorização como onde está a versão codificada `Basic {value}` `value` base 64 de nome de usuário:senha.</span><span class="sxs-lookup"><span data-stu-id="1e0fa-106">The username and password is sent as the Authorization header as `Basic {value}` where `value` is base 64 encoded version of username:password.</span></span>

<span data-ttu-id="1e0fa-107">Herda de [apiAuthenticationConfigurationBase](../resources/apiauthenticationconfigurationbase.md).</span><span class="sxs-lookup"><span data-stu-id="1e0fa-107">Inherits from [apiAuthenticationConfigurationBase](../resources/apiauthenticationconfigurationbase.md).</span></span>

## <a name="properties"></a><span data-ttu-id="1e0fa-108">Propriedades</span><span class="sxs-lookup"><span data-stu-id="1e0fa-108">Properties</span></span>

|<span data-ttu-id="1e0fa-109">Propriedade</span><span class="sxs-lookup"><span data-stu-id="1e0fa-109">Property</span></span>|<span data-ttu-id="1e0fa-110">Tipo</span><span class="sxs-lookup"><span data-stu-id="1e0fa-110">Type</span></span>|<span data-ttu-id="1e0fa-111">Descrição</span><span class="sxs-lookup"><span data-stu-id="1e0fa-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="1e0fa-112">username</span><span class="sxs-lookup"><span data-stu-id="1e0fa-112">username</span></span>|<span data-ttu-id="1e0fa-113">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="1e0fa-113">String</span></span>| <span data-ttu-id="1e0fa-114">O nome de usuário.</span><span class="sxs-lookup"><span data-stu-id="1e0fa-114">The username.</span></span> |
|<span data-ttu-id="1e0fa-115">password</span><span class="sxs-lookup"><span data-stu-id="1e0fa-115">password</span></span>|<span data-ttu-id="1e0fa-116">String</span><span class="sxs-lookup"><span data-stu-id="1e0fa-116">String</span></span>| <span data-ttu-id="1e0fa-117">A senha.</span><span class="sxs-lookup"><span data-stu-id="1e0fa-117">The password.</span></span> <span data-ttu-id="1e0fa-118">Ele não é retornado nas respostas.</span><span class="sxs-lookup"><span data-stu-id="1e0fa-118">It is not returned in the responses.</span></span> |

## <a name="relationships"></a><span data-ttu-id="1e0fa-119">Relações</span><span class="sxs-lookup"><span data-stu-id="1e0fa-119">Relationships</span></span>

<span data-ttu-id="1e0fa-120">Nenhum</span><span class="sxs-lookup"><span data-stu-id="1e0fa-120">None.</span></span>

## <a name="json-representation"></a><span data-ttu-id="1e0fa-121">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="1e0fa-121">JSON representation</span></span>

<span data-ttu-id="1e0fa-122">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="1e0fa-122">The following is a JSON representation of the resource.</span></span>
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
