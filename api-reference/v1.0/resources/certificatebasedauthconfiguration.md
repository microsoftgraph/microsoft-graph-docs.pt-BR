---
title: tipo de recurso certificateBasedAuthConfiguration
description: Representa uma coleção de autoridades de certificação.
localization_priority: Normal
author: davidmu1
ms.prod: microsoft-identity-platform
doc_type: resourcePageType
ms.openlocfilehash: 908a648add1d3e3ea2da4a90fe0f13d2e561ee17
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/05/2020
ms.locfileid: "42531942"
---
# <a name="certificatebasedauthconfiguration-resource-type"></a><span data-ttu-id="d4cb9-103">tipo de recurso certificateBasedAuthConfiguration</span><span class="sxs-lookup"><span data-stu-id="d4cb9-103">certificateBasedAuthConfiguration resource type</span></span>

<span data-ttu-id="d4cb9-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="d4cb9-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="d4cb9-105">A autenticação baseada em certificado permite que você seja autenticado pelo Azure Active Directory com um certificado de cliente em um dispositivo Windows, Android ou iOS ao conectar sua conta do Exchange Online a:</span><span class="sxs-lookup"><span data-stu-id="d4cb9-105">Certificate-based authentication enables you to be authenticated by Azure Active Directory with a client certificate on a Windows, Android, or iOS device when connecting your Exchange Online account to:</span></span>

- <span data-ttu-id="d4cb9-106">Aplicativos móveis da Microsoft, como Outlook e Word</span><span class="sxs-lookup"><span data-stu-id="d4cb9-106">Microsoft mobile applications such as Outlook and Word</span></span>
- <span data-ttu-id="d4cb9-107">Clientes do Exchange ActiveSync (EAS)</span><span class="sxs-lookup"><span data-stu-id="d4cb9-107">Exchange ActiveSync (EAS) clients</span></span>

<span data-ttu-id="d4cb9-108">A configuração desse recurso elimina a necessidade de inserir uma combinação de nome de usuário e senha em determinados emails e aplicativos do Microsoft Office em seu dispositivo móvel.</span><span class="sxs-lookup"><span data-stu-id="d4cb9-108">Configuring this feature eliminates the need to enter a username and password combination into certain mail and Microsoft Office applications on your mobile device.</span></span>

<span data-ttu-id="d4cb9-109">A configuração de autenticação baseada em certificado é fornecida por meio de uma coleção de autoridades de certificação.</span><span class="sxs-lookup"><span data-stu-id="d4cb9-109">Certificate-based authentication configuration is provided through a collection of certificate authorities.</span></span> <span data-ttu-id="d4cb9-110">As autoridades de certificação são usadas para estabelecer uma cadeia de certificados confiáveis que permite que os clientes sejam autenticados pelo Azure Active Directory com um certificado de cliente.</span><span class="sxs-lookup"><span data-stu-id="d4cb9-110">The certificate authorities are used to establish a trusted certificate chain which enables clients to be authenticated by Azure Active Directory with a client certificate.</span></span>

<span data-ttu-id="d4cb9-111">Saiba mais sobre [a autenticação baseada em certificado no Azure Active Directory](https://docs.microsoft.com/azure/active-directory/authentication/active-directory-certificate-based-authentication-get-started).</span><span class="sxs-lookup"><span data-stu-id="d4cb9-111">Learn more about [certificate-based authentication in Azure Active Directory](https://docs.microsoft.com/azure/active-directory/authentication/active-directory-certificate-based-authentication-get-started).</span></span>

## <a name="methods"></a><span data-ttu-id="d4cb9-112">Métodos</span><span class="sxs-lookup"><span data-stu-id="d4cb9-112">Methods</span></span>

| <span data-ttu-id="d4cb9-113">Método</span><span class="sxs-lookup"><span data-stu-id="d4cb9-113">Method</span></span>       | <span data-ttu-id="d4cb9-114">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="d4cb9-114">Return Type</span></span> | <span data-ttu-id="d4cb9-115">Descrição</span><span class="sxs-lookup"><span data-stu-id="d4cb9-115">Description</span></span> |
|:-------------|:------------|:------------|
| [<span data-ttu-id="d4cb9-116">Listar certificateBasedAuthConfiguration</span><span class="sxs-lookup"><span data-stu-id="d4cb9-116">List certificateBasedAuthConfiguration</span></span>](../api/certificatebasedauthconfiguration-list.md) | [<span data-ttu-id="d4cb9-117">certificateBasedAuthConfiguration</span><span class="sxs-lookup"><span data-stu-id="d4cb9-117">certificateBasedAuthConfiguration</span></span>](certificatebasedauthconfiguration.md) | <span data-ttu-id="d4cb9-118">Lista as propriedades da coleção **certificateBasedAuthConfiguration** .</span><span class="sxs-lookup"><span data-stu-id="d4cb9-118">List the properties of the **certificateBasedAuthConfiguration** collection.</span></span> |
| [<span data-ttu-id="d4cb9-119">Criar certificateBasedAuthConfiguration</span><span class="sxs-lookup"><span data-stu-id="d4cb9-119">Create certificateBasedAuthConfiguration</span></span>](../api/certificatebasedauthconfiguration-post-certificatebasedauthconfiguration.md) | [<span data-ttu-id="d4cb9-120">certificateBasedAuthConfiguration</span><span class="sxs-lookup"><span data-stu-id="d4cb9-120">certificateBasedAuthConfiguration</span></span>](certificatebasedauthconfiguration.md) | <span data-ttu-id="d4cb9-121">Criar um novo objeto **certificateBasedAuthConfiguration** .</span><span class="sxs-lookup"><span data-stu-id="d4cb9-121">Create a new **certificateBasedAuthConfiguration** object.</span></span> |
| [<span data-ttu-id="d4cb9-122">Obter certificateBasedAuthConfiguration</span><span class="sxs-lookup"><span data-stu-id="d4cb9-122">Get certificateBasedAuthConfiguration</span></span>](../api/certificatebasedauthconfiguration-get.md) | [<span data-ttu-id="d4cb9-123">certificateBasedAuthConfiguration</span><span class="sxs-lookup"><span data-stu-id="d4cb9-123">certificateBasedAuthConfiguration</span></span>](certificatebasedauthconfiguration.md) | <span data-ttu-id="d4cb9-124">Ler as propriedades de um objeto **certificateBasedAuthConfiguration** .</span><span class="sxs-lookup"><span data-stu-id="d4cb9-124">Read the properties of a **certificateBasedAuthConfiguration** object.</span></span> |
| [<span data-ttu-id="d4cb9-125">Excluir certificateBasedAuthConfiguration</span><span class="sxs-lookup"><span data-stu-id="d4cb9-125">Delete certificateBasedAuthConfiguration</span></span>](../api/certificatebasedauthconfiguration-delete.md) | <span data-ttu-id="d4cb9-126">Nenhum</span><span class="sxs-lookup"><span data-stu-id="d4cb9-126">None</span></span> | <span data-ttu-id="d4cb9-127">Excluir um objeto **certificateBasedAuthConfiguration** .</span><span class="sxs-lookup"><span data-stu-id="d4cb9-127">Delete a **certificateBasedAuthConfiguration** object.</span></span> |

>[!NOTE]
><span data-ttu-id="d4cb9-128">Não há suporte para a atualização de **cerficateBasedAuthConfiguration** .</span><span class="sxs-lookup"><span data-stu-id="d4cb9-128">Updating **cerficateBasedAuthConfiguration** is not supported.</span></span> <span data-ttu-id="d4cb9-129">Para alterar um **cerficateBasedAuthConfiguration**, primeiro exclua e crie um novo **cerficateBasedAuthConfiguration**.</span><span class="sxs-lookup"><span data-stu-id="d4cb9-129">To change a **cerficateBasedAuthConfiguration**, first delete and then create a new **cerficateBasedAuthConfiguration**.</span></span>

## <a name="properties"></a><span data-ttu-id="d4cb9-130">Propriedades</span><span class="sxs-lookup"><span data-stu-id="d4cb9-130">Properties</span></span>

| <span data-ttu-id="d4cb9-131">Propriedade</span><span class="sxs-lookup"><span data-stu-id="d4cb9-131">Property</span></span>     | <span data-ttu-id="d4cb9-132">Tipo</span><span class="sxs-lookup"><span data-stu-id="d4cb9-132">Type</span></span>        | <span data-ttu-id="d4cb9-133">Descrição</span><span class="sxs-lookup"><span data-stu-id="d4cb9-133">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="d4cb9-134">certificateAuthorities</span><span class="sxs-lookup"><span data-stu-id="d4cb9-134">certificateAuthorities</span></span>|<span data-ttu-id="d4cb9-135">coleção [certificateAuthority](certificateauthority.md)</span><span class="sxs-lookup"><span data-stu-id="d4cb9-135">[certificateAuthority](certificateauthority.md) collection</span></span>|<span data-ttu-id="d4cb9-136">Coleção de autoridades de certificação que cria uma cadeia de certificado confiável.</span><span class="sxs-lookup"><span data-stu-id="d4cb9-136">Collection of certificate authorities which creates a trusted certificate chain.</span></span>|
|<span data-ttu-id="d4cb9-137">id</span><span class="sxs-lookup"><span data-stu-id="d4cb9-137">id</span></span>|<span data-ttu-id="d4cb9-138">String</span><span class="sxs-lookup"><span data-stu-id="d4cb9-138">String</span></span>|<span data-ttu-id="d4cb9-139">O identificador exclusivo da configuração de autenticação baseada em certificado.</span><span class="sxs-lookup"><span data-stu-id="d4cb9-139">The unique identifier of the certificate based auth configuration.</span></span> <span data-ttu-id="d4cb9-140">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="d4cb9-140">Read-only.</span></span>|

## <a name="relationships"></a><span data-ttu-id="d4cb9-141">Relações</span><span class="sxs-lookup"><span data-stu-id="d4cb9-141">Relationships</span></span>

<span data-ttu-id="d4cb9-142">Nenhum</span><span class="sxs-lookup"><span data-stu-id="d4cb9-142">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="d4cb9-143">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="d4cb9-143">JSON representation</span></span>

<span data-ttu-id="d4cb9-144">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="d4cb9-144">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.certificateBasedAuthConfiguration",
  "baseType": "",
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
