---
title: Tipo de recurso basicAuthentication
description: Representa a configuração para o uso da autenticação básica em uma chamada de API.
author: nickgmicrosoft
localization_priority: Normal
ms.prod: identity-and-sign-in
doc_type: resourcePageType
ms.openlocfilehash: 396cadec8e1766bee662c51df8d7999ba6a0ba6c
ms.sourcegitcommit: 9d98d9e9cc1e193850ab9b82aaaf906d70e1378b
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/12/2021
ms.locfileid: "50761685"
---
# <a name="basicauthentication-resource-type"></a><span data-ttu-id="37336-103">Tipo de recurso basicAuthentication</span><span class="sxs-lookup"><span data-stu-id="37336-103">basicAuthentication resource type</span></span>

<span data-ttu-id="37336-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="37336-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="37336-105">Representa a configuração para o uso da autenticação HTTP Basic, que envolve um nome de usuário e uma senha, em uma chamada de API.</span><span class="sxs-lookup"><span data-stu-id="37336-105">Represents configuration for using HTTP Basic authentication, which entails a username and password, in an API call.</span></span> <span data-ttu-id="37336-106">O nome de usuário e a senha são enviados como o header de Autorização como onde está a versão codificada `Basic {value}` `value` base 64 de nome de usuário:senha.</span><span class="sxs-lookup"><span data-stu-id="37336-106">The username and password is sent as the Authorization header as `Basic {value}` where `value` is base 64 encoded version of username:password.</span></span>

<span data-ttu-id="37336-107">Herda de [apiAuthenticationConfigurationBase](../resources/apiauthenticationconfigurationbase.md).</span><span class="sxs-lookup"><span data-stu-id="37336-107">Inherits from [apiAuthenticationConfigurationBase](../resources/apiauthenticationconfigurationbase.md).</span></span>

## <a name="properties"></a><span data-ttu-id="37336-108">Propriedades</span><span class="sxs-lookup"><span data-stu-id="37336-108">Properties</span></span>

|<span data-ttu-id="37336-109">Propriedade</span><span class="sxs-lookup"><span data-stu-id="37336-109">Property</span></span>|<span data-ttu-id="37336-110">Tipo</span><span class="sxs-lookup"><span data-stu-id="37336-110">Type</span></span>|<span data-ttu-id="37336-111">Descrição</span><span class="sxs-lookup"><span data-stu-id="37336-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="37336-112">username</span><span class="sxs-lookup"><span data-stu-id="37336-112">username</span></span>|<span data-ttu-id="37336-113">Cadeia de Caracteres</span><span class="sxs-lookup"><span data-stu-id="37336-113">String</span></span>| <span data-ttu-id="37336-114">O nome de usuário.</span><span class="sxs-lookup"><span data-stu-id="37336-114">The username.</span></span> |
|<span data-ttu-id="37336-115">password</span><span class="sxs-lookup"><span data-stu-id="37336-115">password</span></span>|<span data-ttu-id="37336-116">String</span><span class="sxs-lookup"><span data-stu-id="37336-116">String</span></span>| <span data-ttu-id="37336-117">A senha.</span><span class="sxs-lookup"><span data-stu-id="37336-117">The password.</span></span> <span data-ttu-id="37336-118">Ele não é retornado nas respostas.</span><span class="sxs-lookup"><span data-stu-id="37336-118">It is not returned in the responses.</span></span> |

## <a name="relationships"></a><span data-ttu-id="37336-119">Relações</span><span class="sxs-lookup"><span data-stu-id="37336-119">Relationships</span></span>

<span data-ttu-id="37336-120">Nenhum</span><span class="sxs-lookup"><span data-stu-id="37336-120">None.</span></span>

## <a name="json-representation"></a><span data-ttu-id="37336-121">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="37336-121">JSON representation</span></span>

<span data-ttu-id="37336-122">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="37336-122">The following is a JSON representation of the resource.</span></span>
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
