---
title: Tipo de recurso certificateBasedAuthConfiguration
description: Representa uma coleção de autoridades de certificados.
localization_priority: Normal
author: adimitui
ms.prod: identity-and-sign-in
doc_type: resourcePageType
ms.openlocfilehash: 1ff4eb3e7a235a27dc9d58b9b4bd631d0aeaed0f
ms.sourcegitcommit: 3b583d7baa9ae81b796fd30bc24c65d26b2cdf43
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/04/2021
ms.locfileid: "50443143"
---
# <a name="certificatebasedauthconfiguration-resource-type"></a><span data-ttu-id="2ccc5-103">Tipo de recurso certificateBasedAuthConfiguration</span><span class="sxs-lookup"><span data-stu-id="2ccc5-103">certificateBasedAuthConfiguration resource type</span></span>

<span data-ttu-id="2ccc5-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="2ccc5-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="2ccc5-105">A autenticação baseada em certificado permite que você seja autenticado pelo Azure Active Directory com um certificado cliente em um dispositivo Windows, Android ou iOS ao conectar sua conta do Exchange Online a:</span><span class="sxs-lookup"><span data-stu-id="2ccc5-105">Certificate-based authentication enables you to be authenticated by Azure Active Directory with a client certificate on a Windows, Android, or iOS device when connecting your Exchange Online account to:</span></span>

- <span data-ttu-id="2ccc5-106">Aplicativos móveis da Microsoft, como Outlook e Word</span><span class="sxs-lookup"><span data-stu-id="2ccc5-106">Microsoft mobile applications such as Outlook and Word</span></span>
- <span data-ttu-id="2ccc5-107">Exchange ActiveSync clientes (EAS)</span><span class="sxs-lookup"><span data-stu-id="2ccc5-107">Exchange ActiveSync (EAS) clients</span></span>

<span data-ttu-id="2ccc5-108">A configuração desse recurso elimina a necessidade de inserir uma combinação de nome de usuário e senha em determinados aplicativos de email e Microsoft Office em seu dispositivo móvel.</span><span class="sxs-lookup"><span data-stu-id="2ccc5-108">Configuring this feature eliminates the need to enter a username and password combination into certain mail and Microsoft Office applications on your mobile device.</span></span>

<span data-ttu-id="2ccc5-109">A configuração de autenticação baseada em certificado é fornecida por meio de uma coleção de autoridades de certificados.</span><span class="sxs-lookup"><span data-stu-id="2ccc5-109">Certificate-based authentication configuration is provided through a collection of certificate authorities.</span></span> <span data-ttu-id="2ccc5-110">As autoridades de certificado são usadas para estabelecer uma cadeia de certificados confiável que permite que os clientes sejam autenticados pelo Azure Active Directory com um certificado de cliente.</span><span class="sxs-lookup"><span data-stu-id="2ccc5-110">The certificate authorities are used to establish a trusted certificate chain which enables clients to be authenticated by Azure Active Directory with a client certificate.</span></span>

<span data-ttu-id="2ccc5-111">Saiba mais sobre [autenticação baseada em certificado no Azure Active Directory](/azure/active-directory/authentication/active-directory-certificate-based-authentication-get-started).</span><span class="sxs-lookup"><span data-stu-id="2ccc5-111">Learn more about [certificate-based authentication in Azure Active Directory](/azure/active-directory/authentication/active-directory-certificate-based-authentication-get-started).</span></span>

## <a name="methods"></a><span data-ttu-id="2ccc5-112">Methods</span><span class="sxs-lookup"><span data-stu-id="2ccc5-112">Methods</span></span>

| <span data-ttu-id="2ccc5-113">Método</span><span class="sxs-lookup"><span data-stu-id="2ccc5-113">Method</span></span>       | <span data-ttu-id="2ccc5-114">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="2ccc5-114">Return Type</span></span> | <span data-ttu-id="2ccc5-115">Descrição</span><span class="sxs-lookup"><span data-stu-id="2ccc5-115">Description</span></span> |
|:-------------|:------------|:------------|
| [<span data-ttu-id="2ccc5-116">Listar certificateBasedAuthConfiguration</span><span class="sxs-lookup"><span data-stu-id="2ccc5-116">List certificateBasedAuthConfiguration</span></span>](../api/certificatebasedauthconfiguration-list.md) | [<span data-ttu-id="2ccc5-117">certificateBasedAuthConfiguration</span><span class="sxs-lookup"><span data-stu-id="2ccc5-117">certificateBasedAuthConfiguration</span></span>](certificatebasedauthconfiguration.md) | <span data-ttu-id="2ccc5-118">Listar as propriedades da **coleção certificateBasedAuthConfiguration.**</span><span class="sxs-lookup"><span data-stu-id="2ccc5-118">List the properties of the **certificateBasedAuthConfiguration** collection.</span></span> |
| [<span data-ttu-id="2ccc5-119">Obter certificateBasedAuthConfiguration</span><span class="sxs-lookup"><span data-stu-id="2ccc5-119">Get certificateBasedAuthConfiguration</span></span>](../api/certificatebasedauthconfiguration-get.md) | [<span data-ttu-id="2ccc5-120">certificateBasedAuthConfiguration</span><span class="sxs-lookup"><span data-stu-id="2ccc5-120">certificateBasedAuthConfiguration</span></span>](certificatebasedauthconfiguration.md) | <span data-ttu-id="2ccc5-121">Leia as propriedades de **um objeto certificateBasedAuthConfiguration.**</span><span class="sxs-lookup"><span data-stu-id="2ccc5-121">Read the properties of a **certificateBasedAuthConfiguration** object.</span></span> |
| [<span data-ttu-id="2ccc5-122">Criar certificateBasedAuthConfiguration</span><span class="sxs-lookup"><span data-stu-id="2ccc5-122">Create certificateBasedAuthConfiguration</span></span>](../api/certificatebasedauthconfiguration-post-certificatebasedauthconfiguration.md) | [<span data-ttu-id="2ccc5-123">certificateBasedAuthConfiguration</span><span class="sxs-lookup"><span data-stu-id="2ccc5-123">certificateBasedAuthConfiguration</span></span>](certificatebasedauthconfiguration.md) | <span data-ttu-id="2ccc5-124">Crie um novo **objeto certificateBasedAuthConfiguration.**</span><span class="sxs-lookup"><span data-stu-id="2ccc5-124">Create a new **certificateBasedAuthConfiguration** object.</span></span> |
| [<span data-ttu-id="2ccc5-125">Excluir certificateBasedAuthConfiguration</span><span class="sxs-lookup"><span data-stu-id="2ccc5-125">Delete certificateBasedAuthConfiguration</span></span>](../api/certificatebasedauthconfiguration-delete.md) | <span data-ttu-id="2ccc5-126">Nenhum(a)</span><span class="sxs-lookup"><span data-stu-id="2ccc5-126">None</span></span> | <span data-ttu-id="2ccc5-127">**Exclua um objeto certificateBasedAuthConfiguration.**</span><span class="sxs-lookup"><span data-stu-id="2ccc5-127">Delete a **certificateBasedAuthConfiguration** object.</span></span> |

>[!NOTE]
><span data-ttu-id="2ccc5-128">Não há suporte para a atualização do cerficateBasedAuthConfiguration.</span><span class="sxs-lookup"><span data-stu-id="2ccc5-128">Updating cerficateBasedAuthConfiguration is not supported.</span></span> <span data-ttu-id="2ccc5-129">Para alterar um cerficateBasedAuthConfiguration, primeiro exclua e crie um novo cerficateBasedAuthConfiguration.</span><span class="sxs-lookup"><span data-stu-id="2ccc5-129">To change a cerficateBasedAuthConfiguration, first delete and then create a new cerficateBasedAuthConfiguration.</span></span>

## <a name="properties"></a><span data-ttu-id="2ccc5-130">Propriedades</span><span class="sxs-lookup"><span data-stu-id="2ccc5-130">Properties</span></span>

| <span data-ttu-id="2ccc5-131">Propriedade</span><span class="sxs-lookup"><span data-stu-id="2ccc5-131">Property</span></span>     | <span data-ttu-id="2ccc5-132">Tipo</span><span class="sxs-lookup"><span data-stu-id="2ccc5-132">Type</span></span>        | <span data-ttu-id="2ccc5-133">Descrição</span><span class="sxs-lookup"><span data-stu-id="2ccc5-133">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="2ccc5-134">certificateAuthorities</span><span class="sxs-lookup"><span data-stu-id="2ccc5-134">certificateAuthorities</span></span>|<span data-ttu-id="2ccc5-135">[Coleção certificateAuthority](certificateauthority.md)</span><span class="sxs-lookup"><span data-stu-id="2ccc5-135">[certificateAuthority](certificateauthority.md) collection</span></span>|<span data-ttu-id="2ccc5-136">Coleção de autoridades de certificados que cria uma cadeia de certificados confiável.</span><span class="sxs-lookup"><span data-stu-id="2ccc5-136">Collection of certificate authorities which creates a trusted certificate chain.</span></span>|
|<span data-ttu-id="2ccc5-137">id</span><span class="sxs-lookup"><span data-stu-id="2ccc5-137">id</span></span>|<span data-ttu-id="2ccc5-138">String</span><span class="sxs-lookup"><span data-stu-id="2ccc5-138">String</span></span>|<span data-ttu-id="2ccc5-139">O identificador exclusivo da configuração de auth baseada em certificado.</span><span class="sxs-lookup"><span data-stu-id="2ccc5-139">The unique identifier of the certificate based auth configuration.</span></span> <span data-ttu-id="2ccc5-140">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="2ccc5-140">Read-only.</span></span>|

## <a name="relationships"></a><span data-ttu-id="2ccc5-141">Relações</span><span class="sxs-lookup"><span data-stu-id="2ccc5-141">Relationships</span></span>

<span data-ttu-id="2ccc5-142">Nenhum</span><span class="sxs-lookup"><span data-stu-id="2ccc5-142">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="2ccc5-143">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="2ccc5-143">JSON representation</span></span>

<span data-ttu-id="2ccc5-144">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="2ccc5-144">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.certificateBasedAuthConfiguration",
  "keyProperty": "id"
}-->

```json
{
  "certificateAuthorities": {"@odata.type": "collection(microsoft.graph.certificateAuthority)"},
  "id": "String (identifier)"
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "certificateBasedAuthConfiguration resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
