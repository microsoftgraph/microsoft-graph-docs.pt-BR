---
title: Tipo de recurso authenticationSourceFilter
description: Filtrar com base na origem da autenticação que é usada para determinar se o ouvinte é executado ou não.
author: jkdouglas
localization_priority: Normal
ms.prod: identity-and-sign-in
doc_type: resourcePageType
ms.openlocfilehash: 4736be415faab65c6ce3b572a1273a73c707ee43
ms.sourcegitcommit: 1004835b44271f2e50332a1bdc9097d4b06a914a
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 02/06/2021
ms.locfileid: "50128628"
---
# <a name="authenticationsourcefilter-resource-type"></a><span data-ttu-id="4a8bf-103">Tipo de recurso authenticationSourceFilter</span><span class="sxs-lookup"><span data-stu-id="4a8bf-103">authenticationSourceFilter resource type</span></span>

<span data-ttu-id="4a8bf-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="4a8bf-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="4a8bf-105">Filtrar com base na origem da autenticação usada para determinar se o ouvinte é avaliado.</span><span class="sxs-lookup"><span data-stu-id="4a8bf-105">Filter based on the source of the authentication that is used to determine whether the listener is evaluated.</span></span>

<span data-ttu-id="4a8bf-106">A **propriedade includeApplications** pode ser usada para habilitar a inscrição self-service em um aplicativo no Azure Active Directory.</span><span class="sxs-lookup"><span data-stu-id="4a8bf-106">The **includeApplications** property can be used to enable self-service sign up on an application in Azure Active Directory.</span></span> <span data-ttu-id="4a8bf-107">Saiba mais lendo a nossa documentação para [habilenciar aplicativos em um fluxo de usuário de inscrição de autoatendenciamento.](https://docs.microsoft.com/azure/active-directory/external-identities/self-service-sign-up-user-flow#add-applications-to-the-self-service-sign-up-user-flow)</span><span class="sxs-lookup"><span data-stu-id="4a8bf-107">Learn more by reading our documentation for [enabling applications in a self-service sign up user flow](https://docs.microsoft.com/azure/active-directory/external-identities/self-service-sign-up-user-flow#add-applications-to-the-self-service-sign-up-user-flow).</span></span>

## <a name="properties"></a><span data-ttu-id="4a8bf-108">Propriedades</span><span class="sxs-lookup"><span data-stu-id="4a8bf-108">Properties</span></span>

|<span data-ttu-id="4a8bf-109">Propriedade</span><span class="sxs-lookup"><span data-stu-id="4a8bf-109">Property</span></span>|<span data-ttu-id="4a8bf-110">Tipo</span><span class="sxs-lookup"><span data-stu-id="4a8bf-110">Type</span></span>|<span data-ttu-id="4a8bf-111">Descrição</span><span class="sxs-lookup"><span data-stu-id="4a8bf-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="4a8bf-112">includeApplications</span><span class="sxs-lookup"><span data-stu-id="4a8bf-112">includeApplications</span></span>|<span data-ttu-id="4a8bf-113">Coleção de cadeias de caracteres</span><span class="sxs-lookup"><span data-stu-id="4a8bf-113">String collection</span></span>|<span data-ttu-id="4a8bf-114">Aplicativos a incluir para avaliação [da authenticationListener](../resources/authenticationlistener.md).</span><span class="sxs-lookup"><span data-stu-id="4a8bf-114">Applications to include for evaluation of the [authenticationListener](../resources/authenticationlistener.md).</span></span> <span data-ttu-id="4a8bf-115">Esses aplicativos acionam a ação associada quando usada como o aplicativo cliente no fluxo de autenticação.</span><span class="sxs-lookup"><span data-stu-id="4a8bf-115">These applications trigger the associated action when used as the client application in the authentication flow.</span></span> <span data-ttu-id="4a8bf-116">O identificador do aplicativo é a ID do cliente do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="4a8bf-116">The application identifer is the application's client id.</span></span>|

## <a name="relationships"></a><span data-ttu-id="4a8bf-117">Relações</span><span class="sxs-lookup"><span data-stu-id="4a8bf-117">Relationships</span></span>

<span data-ttu-id="4a8bf-118">Nenhum</span><span class="sxs-lookup"><span data-stu-id="4a8bf-118">None.</span></span>

## <a name="json-representation"></a><span data-ttu-id="4a8bf-119">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="4a8bf-119">JSON representation</span></span>

<span data-ttu-id="4a8bf-120">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="4a8bf-120">The following is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.authenticationSourceFilter"
}
-->

``` json
{
  "@odata.type": "#microsoft.graph.authenticationSourceFilter",
  "includeApplications": [
    "String"
  ]
}
```
