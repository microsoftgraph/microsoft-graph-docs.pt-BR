---
title: Tipo de recurso certificateBasedAuthConfiguration
description: Representa uma coleção de autoridades de certificação.
localization_priority: Normal
author: adimitui
ms.prod: microsoft-identity-platform
doc_type: resourcePageType
ms.openlocfilehash: 0fcc5f37cb55ad0cc5e9e76bf0fe7efb6c4ab517
ms.sourcegitcommit: eb31a6b4a582a59b44df3453450a82fd366342d0
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 02/09/2021
ms.locfileid: "50153477"
---
# <a name="certificatebasedauthconfiguration-resource-type"></a><span data-ttu-id="78f62-103">Tipo de recurso certificateBasedAuthConfiguration</span><span class="sxs-lookup"><span data-stu-id="78f62-103">certificateBasedAuthConfiguration resource type</span></span>

<span data-ttu-id="78f62-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="78f62-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="78f62-105">A autenticação baseada em certificado permite que você seja autenticado pelo Azure Active Directory com um certificado de cliente em um dispositivo Windows, Android ou iOS ao conectar sua conta do Exchange Online a:</span><span class="sxs-lookup"><span data-stu-id="78f62-105">Certificate-based authentication enables you to be authenticated by Azure Active Directory with a client certificate on a Windows, Android, or iOS device when connecting your Exchange Online account to:</span></span>

- <span data-ttu-id="78f62-106">Aplicativos móveis da Microsoft, como o Outlook e o Word</span><span class="sxs-lookup"><span data-stu-id="78f62-106">Microsoft mobile applications such as Outlook and Word</span></span>
- <span data-ttu-id="78f62-107">Clientes do Exchange ActiveSync (EAS)</span><span class="sxs-lookup"><span data-stu-id="78f62-107">Exchange ActiveSync (EAS) clients</span></span>

<span data-ttu-id="78f62-108">A configuração desse recurso elimina a necessidade de inserir uma combinação de nome de usuário e senha em determinados aplicativos de email e do Microsoft Office em seu dispositivo móvel.</span><span class="sxs-lookup"><span data-stu-id="78f62-108">Configuring this feature eliminates the need to enter a username and password combination into certain mail and Microsoft Office applications on your mobile device.</span></span>

<span data-ttu-id="78f62-109">A configuração de autenticação baseada em certificado é fornecida por meio de um conjunto de autoridades de certificação.</span><span class="sxs-lookup"><span data-stu-id="78f62-109">Certificate-based authentication configuration is provided through a collection of certificate authorities.</span></span> <span data-ttu-id="78f62-110">As autoridades de certificação são usadas para estabelecer uma cadeia de certificados confiável que permite que os clientes sejam autenticados pelo Azure Active Directory com um certificado de cliente.</span><span class="sxs-lookup"><span data-stu-id="78f62-110">The certificate authorities are used to establish a trusted certificate chain which enables clients to be authenticated by Azure Active Directory with a client certificate.</span></span>

<span data-ttu-id="78f62-111">Saiba mais sobre [a autenticação baseada em certificado no Azure Active Directory.](/azure/active-directory/authentication/active-directory-certificate-based-authentication-get-started)</span><span class="sxs-lookup"><span data-stu-id="78f62-111">Learn more about [certificate-based authentication in Azure Active Directory](/azure/active-directory/authentication/active-directory-certificate-based-authentication-get-started).</span></span>

## <a name="methods"></a><span data-ttu-id="78f62-112">Métodos</span><span class="sxs-lookup"><span data-stu-id="78f62-112">Methods</span></span>

| <span data-ttu-id="78f62-113">Método</span><span class="sxs-lookup"><span data-stu-id="78f62-113">Method</span></span>       | <span data-ttu-id="78f62-114">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="78f62-114">Return Type</span></span> | <span data-ttu-id="78f62-115">Descrição</span><span class="sxs-lookup"><span data-stu-id="78f62-115">Description</span></span> |
|:-------------|:------------|:------------|
| [<span data-ttu-id="78f62-116">Listar certificateBasedAuthConfiguration</span><span class="sxs-lookup"><span data-stu-id="78f62-116">List certificateBasedAuthConfiguration</span></span>](../api/certificatebasedauthconfiguration-list.md) | [<span data-ttu-id="78f62-117">certificateBasedAuthConfiguration</span><span class="sxs-lookup"><span data-stu-id="78f62-117">certificateBasedAuthConfiguration</span></span>](certificatebasedauthconfiguration.md) | <span data-ttu-id="78f62-118">Listar as propriedades da **coleção certificateBasedAuthConfiguration.**</span><span class="sxs-lookup"><span data-stu-id="78f62-118">List the properties of the **certificateBasedAuthConfiguration** collection.</span></span> |
| [<span data-ttu-id="78f62-119">Criar certificateBasedAuthConfiguration</span><span class="sxs-lookup"><span data-stu-id="78f62-119">Create certificateBasedAuthConfiguration</span></span>](../api/certificatebasedauthconfiguration-post-certificatebasedauthconfiguration.md) | [<span data-ttu-id="78f62-120">certificateBasedAuthConfiguration</span><span class="sxs-lookup"><span data-stu-id="78f62-120">certificateBasedAuthConfiguration</span></span>](certificatebasedauthconfiguration.md) | <span data-ttu-id="78f62-121">Criar um novo **objeto certificateBasedAuthConfiguration.**</span><span class="sxs-lookup"><span data-stu-id="78f62-121">Create a new **certificateBasedAuthConfiguration** object.</span></span> |
| [<span data-ttu-id="78f62-122">Obter certificateBasedAuthConfiguration</span><span class="sxs-lookup"><span data-stu-id="78f62-122">Get certificateBasedAuthConfiguration</span></span>](../api/certificatebasedauthconfiguration-get.md) | [<span data-ttu-id="78f62-123">certificateBasedAuthConfiguration</span><span class="sxs-lookup"><span data-stu-id="78f62-123">certificateBasedAuthConfiguration</span></span>](certificatebasedauthconfiguration.md) | <span data-ttu-id="78f62-124">Leia as propriedades de um **objeto certificateBasedAuthConfiguration.**</span><span class="sxs-lookup"><span data-stu-id="78f62-124">Read the properties of a **certificateBasedAuthConfiguration** object.</span></span> |
| [<span data-ttu-id="78f62-125">Excluir certificateBasedAuthConfiguration</span><span class="sxs-lookup"><span data-stu-id="78f62-125">Delete certificateBasedAuthConfiguration</span></span>](../api/certificatebasedauthconfiguration-delete.md) | <span data-ttu-id="78f62-126">Nenhum</span><span class="sxs-lookup"><span data-stu-id="78f62-126">None</span></span> | <span data-ttu-id="78f62-127">**Exclua um objeto certificateBasedAuthConfiguration.**</span><span class="sxs-lookup"><span data-stu-id="78f62-127">Delete a **certificateBasedAuthConfiguration** object.</span></span> |

>[!NOTE]
><span data-ttu-id="78f62-128">Não há suporte para a atualização de **certificateBasedAuthConfiguration.**</span><span class="sxs-lookup"><span data-stu-id="78f62-128">Updating **certificateBasedAuthConfiguration** is not supported.</span></span> <span data-ttu-id="78f62-129">Para alterar um **certificateBasedAuthConfiguration**, primeiro exclua e depois crie um novo **certificateBasedAuthConfiguration**.</span><span class="sxs-lookup"><span data-stu-id="78f62-129">To change a **certificateBasedAuthConfiguration**, first delete and then create a new **certificateBasedAuthConfiguration**.</span></span>

## <a name="properties"></a><span data-ttu-id="78f62-130">Propriedades</span><span class="sxs-lookup"><span data-stu-id="78f62-130">Properties</span></span>

| <span data-ttu-id="78f62-131">Propriedade</span><span class="sxs-lookup"><span data-stu-id="78f62-131">Property</span></span>     | <span data-ttu-id="78f62-132">Tipo</span><span class="sxs-lookup"><span data-stu-id="78f62-132">Type</span></span>        | <span data-ttu-id="78f62-133">Descrição</span><span class="sxs-lookup"><span data-stu-id="78f62-133">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="78f62-134">certificateAuthorities</span><span class="sxs-lookup"><span data-stu-id="78f62-134">certificateAuthorities</span></span>|<span data-ttu-id="78f62-135">[Coleção certificateAuthority](certificateauthority.md)</span><span class="sxs-lookup"><span data-stu-id="78f62-135">[certificateAuthority](certificateauthority.md) collection</span></span>|<span data-ttu-id="78f62-136">Coleção de autoridades de certificação que cria uma cadeia de certificados confiáveis.</span><span class="sxs-lookup"><span data-stu-id="78f62-136">Collection of certificate authorities which creates a trusted certificate chain.</span></span>|
|<span data-ttu-id="78f62-137">id</span><span class="sxs-lookup"><span data-stu-id="78f62-137">id</span></span>|<span data-ttu-id="78f62-138">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="78f62-138">String</span></span>|<span data-ttu-id="78f62-139">O identificador exclusivo da configuração de auth baseada em certificado.</span><span class="sxs-lookup"><span data-stu-id="78f62-139">The unique identifier of the certificate based auth configuration.</span></span> <span data-ttu-id="78f62-140">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="78f62-140">Read-only.</span></span>|

## <a name="relationships"></a><span data-ttu-id="78f62-141">Relações</span><span class="sxs-lookup"><span data-stu-id="78f62-141">Relationships</span></span>

<span data-ttu-id="78f62-142">Nenhum,</span><span class="sxs-lookup"><span data-stu-id="78f62-142">None,</span></span>

## <a name="json-representation"></a><span data-ttu-id="78f62-143">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="78f62-143">JSON representation</span></span>

<span data-ttu-id="78f62-144">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="78f62-144">The following is a JSON representation of the resource.</span></span>

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
