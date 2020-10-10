---
title: tipo de recurso passwordlessMicrosoftAuthenticatorAuthenticationMethod
description: Uma representação de um método de entrada de telefone sem senha do autenticador da Microsoft registrado para um usuário.
author: mmcla
localization_priority: Normal
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: b34b807106591390198c58d26d7804dc6ada5460
ms.sourcegitcommit: cfadc605014265e02b913bc77382025b0d156285
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 10/10/2020
ms.locfileid: "48418206"
---
# <a name="passwordlessmicrosoftauthenticatorauthenticationmethod-resource-type"></a><span data-ttu-id="8e3f1-103">tipo de recurso passwordlessMicrosoftAuthenticatorAuthenticationMethod</span><span class="sxs-lookup"><span data-stu-id="8e3f1-103">passwordlessMicrosoftAuthenticatorAuthenticationMethod resource type</span></span>

<span data-ttu-id="8e3f1-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="8e3f1-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="8e3f1-105">Uma representação de um método de entrada de telefone sem senha do autenticador da Microsoft registrado para um usuário.</span><span class="sxs-lookup"><span data-stu-id="8e3f1-105">A representation of a Microsoft Authenticator Passwordless Phone Sign-in method registered to a user.</span></span>

> [!NOTE]
> <span data-ttu-id="8e3f1-106">Alterações substanciais de esquema são planejadas para APIs que gerenciam o aplicativo Microsoft Authenticator enquanto as APIs estão no Mirosoft Graph beta.</span><span class="sxs-lookup"><span data-stu-id="8e3f1-106">Substantial schema changes are planned for APIs that manage the Microsoft Authenticator app while the APIs are in Mirosoft Graph beta.</span></span> <span data-ttu-id="8e3f1-107">Como os padrões de chamada serão alterados, recomendamos que você não faça uma dependência de produção nessas APIs.</span><span class="sxs-lookup"><span data-stu-id="8e3f1-107">Because the calling patterns will change, we recommend that you do not take a production dependency on these APIs.</span></span>


## <a name="methods"></a><span data-ttu-id="8e3f1-108">Métodos</span><span class="sxs-lookup"><span data-stu-id="8e3f1-108">Methods</span></span>
|<span data-ttu-id="8e3f1-109">Método</span><span class="sxs-lookup"><span data-stu-id="8e3f1-109">Method</span></span>|<span data-ttu-id="8e3f1-110">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="8e3f1-110">Return type</span></span>|<span data-ttu-id="8e3f1-111">Descrição</span><span class="sxs-lookup"><span data-stu-id="8e3f1-111">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="8e3f1-112">List</span><span class="sxs-lookup"><span data-stu-id="8e3f1-112">List</span></span>](../api/passwordlessmicrosoftauthenticatorauthenticationmethod-list.md)|<span data-ttu-id="8e3f1-113">coleção [passwordlessMicrosoftAuthenticatorAuthenticationMethod](../resources/passwordlessmicrosoftauthenticatorauthenticationmethod.md)</span><span class="sxs-lookup"><span data-stu-id="8e3f1-113">[passwordlessMicrosoftAuthenticatorAuthenticationMethod](../resources/passwordlessmicrosoftauthenticatorauthenticationmethod.md) collection</span></span>|<span data-ttu-id="8e3f1-114">Recupere uma lista de objetos passwordlessMicrosoftAuthenticatorAuthenticationMethod de um usuário e suas propriedades.</span><span class="sxs-lookup"><span data-stu-id="8e3f1-114">Retrieve a list of a user's passwordlessMicrosoftAuthenticatorAuthenticationMethod objects and their properties.</span></span>|
|[<span data-ttu-id="8e3f1-115">Obter</span><span class="sxs-lookup"><span data-stu-id="8e3f1-115">Get</span></span>](../api/passwordlessmicrosoftauthenticatorauthenticationmethod-get.md)|[<span data-ttu-id="8e3f1-116">passwordlessMicrosoftAuthenticatorAuthenticationMethod</span><span class="sxs-lookup"><span data-stu-id="8e3f1-116">passwordlessMicrosoftAuthenticatorAuthenticationMethod</span></span>](../resources/passwordlessmicrosoftauthenticatorauthenticationmethod.md)|<span data-ttu-id="8e3f1-117">Leia as propriedades e os relacionamentos do objeto passwordlessMicrosoftAuthenticatorAuthenticationMethod de um usuário.</span><span class="sxs-lookup"><span data-stu-id="8e3f1-117">Read the properties and relationships of a user's passwordlessMicrosoftAuthenticatorAuthenticationMethod object.</span></span>|
|[<span data-ttu-id="8e3f1-118">Excluir</span><span class="sxs-lookup"><span data-stu-id="8e3f1-118">Delete</span></span>](../api/passwordlessmicrosoftauthenticatorauthenticationmethod-delete.md)|<span data-ttu-id="8e3f1-119">Nenhum</span><span class="sxs-lookup"><span data-stu-id="8e3f1-119">None</span></span>|<span data-ttu-id="8e3f1-120">Exclui o objeto passwordlessMicrosoftAuthenticatorAuthenticationMethod de um usuário.</span><span class="sxs-lookup"><span data-stu-id="8e3f1-120">Deletes a user's passwordlessMicrosoftAuthenticatorAuthenticationMethod object.</span></span>|


## <a name="properties"></a><span data-ttu-id="8e3f1-121">Propriedades</span><span class="sxs-lookup"><span data-stu-id="8e3f1-121">Properties</span></span>
|<span data-ttu-id="8e3f1-122">Propriedade</span><span class="sxs-lookup"><span data-stu-id="8e3f1-122">Property</span></span>|<span data-ttu-id="8e3f1-123">Tipo</span><span class="sxs-lookup"><span data-stu-id="8e3f1-123">Type</span></span>|<span data-ttu-id="8e3f1-124">Descrição</span><span class="sxs-lookup"><span data-stu-id="8e3f1-124">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="8e3f1-125">id</span><span class="sxs-lookup"><span data-stu-id="8e3f1-125">id</span></span>|<span data-ttu-id="8e3f1-126">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="8e3f1-126">String</span></span>|<span data-ttu-id="8e3f1-127">O identificador do método de autenticação.</span><span class="sxs-lookup"><span data-stu-id="8e3f1-127">The authentication method identifier.</span></span>|
|<span data-ttu-id="8e3f1-128">displayName</span><span class="sxs-lookup"><span data-stu-id="8e3f1-128">displayName</span></span>|<span data-ttu-id="8e3f1-129">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="8e3f1-129">String</span></span>|<span data-ttu-id="8e3f1-130">O nome de exibição do dispositivo móvel conforme fornecido pelo usuário.</span><span class="sxs-lookup"><span data-stu-id="8e3f1-130">The display name of the mobile device as given by the user.</span></span>|
|<span data-ttu-id="8e3f1-131">creationDatetime</span><span class="sxs-lookup"><span data-stu-id="8e3f1-131">creationDateTime</span></span>|<span data-ttu-id="8e3f1-132">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="8e3f1-132">DateTimeOffset</span></span>|<span data-ttu-id="8e3f1-133">O carimbo de data/hora em que esse método foi registrado para o usuário.</span><span class="sxs-lookup"><span data-stu-id="8e3f1-133">The timestamp when this method was registered to the user.</span></span>|


## <a name="json-representation"></a><span data-ttu-id="8e3f1-134">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="8e3f1-134">JSON representation</span></span>
<span data-ttu-id="8e3f1-135">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="8e3f1-135">The following is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.passwordlessMicrosoftAuthenticatorAuthenticationMethod",
  "baseType": "microsoft.graph.authenticationMethod",
  "openType": false
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.passwordlessMicrosoftAuthenticatorAuthenticationMethod",
  "id": "String (identifier)",
  "displayName": "String",
  "creationDateTime": "String (timestamp)"
}
```

