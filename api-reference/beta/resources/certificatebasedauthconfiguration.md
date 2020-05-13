---
title: tipo de recurso certificateBasedAuthConfiguration
description: Representa uma coleção de autoridades de certificação.
localization_priority: Normal
author: adimitui
ms.prod: microsoft-identity-platform
doc_type: resourcePageType
ms.openlocfilehash: b834de13ccfeb59cd88fae093406a380c9aa5b58
ms.sourcegitcommit: d4114bac58628527611e83e436132c6581a19c52
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/13/2020
ms.locfileid: "43181789"
---
# <a name="certificatebasedauthconfiguration-resource-type"></a><span data-ttu-id="3e37e-103">tipo de recurso certificateBasedAuthConfiguration</span><span class="sxs-lookup"><span data-stu-id="3e37e-103">certificateBasedAuthConfiguration resource type</span></span>

<span data-ttu-id="3e37e-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="3e37e-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="3e37e-105">A autenticação baseada em certificado permite que você seja autenticado pelo Azure Active Directory com um certificado de cliente em um dispositivo Windows, Android ou iOS ao conectar sua conta do Exchange Online a:</span><span class="sxs-lookup"><span data-stu-id="3e37e-105">Certificate-based authentication enables you to be authenticated by Azure Active Directory with a client certificate on a Windows, Android, or iOS device when connecting your Exchange Online account to:</span></span>

- <span data-ttu-id="3e37e-106">Aplicativos móveis da Microsoft, como Outlook e Word</span><span class="sxs-lookup"><span data-stu-id="3e37e-106">Microsoft mobile applications such as Outlook and Word</span></span>
- <span data-ttu-id="3e37e-107">Clientes do Exchange ActiveSync (EAS)</span><span class="sxs-lookup"><span data-stu-id="3e37e-107">Exchange ActiveSync (EAS) clients</span></span>

<span data-ttu-id="3e37e-108">A configuração desse recurso elimina a necessidade de inserir uma combinação de nome de usuário e senha em determinados emails e aplicativos do Microsoft Office em seu dispositivo móvel.</span><span class="sxs-lookup"><span data-stu-id="3e37e-108">Configuring this feature eliminates the need to enter a username and password combination into certain mail and Microsoft Office applications on your mobile device.</span></span>

<span data-ttu-id="3e37e-109">A configuração de autenticação baseada em certificado é fornecida por meio de uma coleção de autoridades de certificação.</span><span class="sxs-lookup"><span data-stu-id="3e37e-109">Certificate-based authentication configuration is provided through a collection of certificate authorities.</span></span> <span data-ttu-id="3e37e-110">As autoridades de certificação são usadas para estabelecer uma cadeia de certificados confiáveis que permite que os clientes sejam autenticados pelo Azure Active Directory com um certificado de cliente.</span><span class="sxs-lookup"><span data-stu-id="3e37e-110">The certificate authorities are used to establish a trusted certificate chain which enables clients to be authenticated by Azure Active Directory with a client certificate.</span></span>

<span data-ttu-id="3e37e-111">Saiba mais sobre [a autenticação baseada em certificado no Azure Active Directory](https://docs.microsoft.com/azure/active-directory/authentication/active-directory-certificate-based-authentication-get-started).</span><span class="sxs-lookup"><span data-stu-id="3e37e-111">Learn more about [certificate-based authentication in Azure Active Directory](https://docs.microsoft.com/azure/active-directory/authentication/active-directory-certificate-based-authentication-get-started).</span></span>

## <a name="methods"></a><span data-ttu-id="3e37e-112">Methods</span><span class="sxs-lookup"><span data-stu-id="3e37e-112">Methods</span></span>

| <span data-ttu-id="3e37e-113">Método</span><span class="sxs-lookup"><span data-stu-id="3e37e-113">Method</span></span>       | <span data-ttu-id="3e37e-114">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="3e37e-114">Return Type</span></span> | <span data-ttu-id="3e37e-115">Descrição</span><span class="sxs-lookup"><span data-stu-id="3e37e-115">Description</span></span> |
|:-------------|:------------|:------------|
| [<span data-ttu-id="3e37e-116">Listar certificateBasedAuthConfiguration</span><span class="sxs-lookup"><span data-stu-id="3e37e-116">List certificateBasedAuthConfiguration</span></span>](../api/certificatebasedauthconfiguration-list.md) | [<span data-ttu-id="3e37e-117">certificateBasedAuthConfiguration</span><span class="sxs-lookup"><span data-stu-id="3e37e-117">certificateBasedAuthConfiguration</span></span>](certificatebasedauthconfiguration.md) | <span data-ttu-id="3e37e-118">Lista as propriedades da coleção **certificateBasedAuthConfiguration** .</span><span class="sxs-lookup"><span data-stu-id="3e37e-118">List the properties of the **certificateBasedAuthConfiguration** collection.</span></span> |
| [<span data-ttu-id="3e37e-119">Obter certificateBasedAuthConfiguration</span><span class="sxs-lookup"><span data-stu-id="3e37e-119">Get certificateBasedAuthConfiguration</span></span>](../api/certificatebasedauthconfiguration-get.md) | [<span data-ttu-id="3e37e-120">certificateBasedAuthConfiguration</span><span class="sxs-lookup"><span data-stu-id="3e37e-120">certificateBasedAuthConfiguration</span></span>](certificatebasedauthconfiguration.md) | <span data-ttu-id="3e37e-121">Ler as propriedades de um objeto **certificateBasedAuthConfiguration** .</span><span class="sxs-lookup"><span data-stu-id="3e37e-121">Read the properties of a **certificateBasedAuthConfiguration** object.</span></span> |
| [<span data-ttu-id="3e37e-122">Criar certificateBasedAuthConfiguration</span><span class="sxs-lookup"><span data-stu-id="3e37e-122">Create certificateBasedAuthConfiguration</span></span>](../api/certificatebasedauthconfiguration-post-certificatebasedauthconfiguration.md) | [<span data-ttu-id="3e37e-123">certificateBasedAuthConfiguration</span><span class="sxs-lookup"><span data-stu-id="3e37e-123">certificateBasedAuthConfiguration</span></span>](certificatebasedauthconfiguration.md) | <span data-ttu-id="3e37e-124">Criar um novo objeto **certificateBasedAuthConfiguration** .</span><span class="sxs-lookup"><span data-stu-id="3e37e-124">Create a new **certificateBasedAuthConfiguration** object.</span></span> |
| [<span data-ttu-id="3e37e-125">Excluir certificateBasedAuthConfiguration</span><span class="sxs-lookup"><span data-stu-id="3e37e-125">Delete certificateBasedAuthConfiguration</span></span>](../api/certificatebasedauthconfiguration-delete.md) | <span data-ttu-id="3e37e-126">Nenhum</span><span class="sxs-lookup"><span data-stu-id="3e37e-126">None</span></span> | <span data-ttu-id="3e37e-127">Excluir um objeto **certificateBasedAuthConfiguration** .</span><span class="sxs-lookup"><span data-stu-id="3e37e-127">Delete a **certificateBasedAuthConfiguration** object.</span></span> |

>[!NOTE]
><span data-ttu-id="3e37e-128">Não há suporte para a atualização de cerficateBasedAuthConfiguration.</span><span class="sxs-lookup"><span data-stu-id="3e37e-128">Updating cerficateBasedAuthConfiguration is not supported.</span></span> <span data-ttu-id="3e37e-129">Para alterar um cerficateBasedAuthConfiguration, primeiro exclua e crie um novo cerficateBasedAuthConfiguration.</span><span class="sxs-lookup"><span data-stu-id="3e37e-129">To change a cerficateBasedAuthConfiguration, first delete and then create a new cerficateBasedAuthConfiguration.</span></span>

## <a name="properties"></a><span data-ttu-id="3e37e-130">Propriedades</span><span class="sxs-lookup"><span data-stu-id="3e37e-130">Properties</span></span>

| <span data-ttu-id="3e37e-131">Propriedade</span><span class="sxs-lookup"><span data-stu-id="3e37e-131">Property</span></span>     | <span data-ttu-id="3e37e-132">Tipo</span><span class="sxs-lookup"><span data-stu-id="3e37e-132">Type</span></span>        | <span data-ttu-id="3e37e-133">Descrição</span><span class="sxs-lookup"><span data-stu-id="3e37e-133">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="3e37e-134">certificateAuthorities</span><span class="sxs-lookup"><span data-stu-id="3e37e-134">certificateAuthorities</span></span>|<span data-ttu-id="3e37e-135">coleção [certificateAuthority](certificateauthority.md)</span><span class="sxs-lookup"><span data-stu-id="3e37e-135">[certificateAuthority](certificateauthority.md) collection</span></span>|<span data-ttu-id="3e37e-136">Coleção de autoridades de certificação que cria uma cadeia de certificado confiável.</span><span class="sxs-lookup"><span data-stu-id="3e37e-136">Collection of certificate authorities which creates a trusted certificate chain.</span></span>|
|<span data-ttu-id="3e37e-137">id</span><span class="sxs-lookup"><span data-stu-id="3e37e-137">id</span></span>|<span data-ttu-id="3e37e-138">String</span><span class="sxs-lookup"><span data-stu-id="3e37e-138">String</span></span>|<span data-ttu-id="3e37e-139">O identificador exclusivo da configuração de autenticação baseada em certificado.</span><span class="sxs-lookup"><span data-stu-id="3e37e-139">The unique identifier of the certificate based auth configuration.</span></span> <span data-ttu-id="3e37e-140">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="3e37e-140">Read-only.</span></span>|

## <a name="relationships"></a><span data-ttu-id="3e37e-141">Relações</span><span class="sxs-lookup"><span data-stu-id="3e37e-141">Relationships</span></span>

<span data-ttu-id="3e37e-142">Nenhum</span><span class="sxs-lookup"><span data-stu-id="3e37e-142">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="3e37e-143">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="3e37e-143">JSON representation</span></span>

<span data-ttu-id="3e37e-144">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="3e37e-144">The following is a JSON representation of the resource.</span></span>

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
