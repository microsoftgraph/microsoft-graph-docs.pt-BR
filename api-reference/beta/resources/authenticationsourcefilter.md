---
title: tipo de recurso authenticationSourceFilter
description: Filtro com base na origem da autenticação que é usada para determinar se o ouvinte foi executado ou não.
author: jkdouglas
localization_priority: Normal
ms.prod: microsoft-identity-platform
doc_type: resourcePageType
ms.openlocfilehash: 0fcbeb3296b6b0dece1b69cedf26d600c240d43d
ms.sourcegitcommit: 424735f8ab46de76b9d850e10c7d97ffd164f62a
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 12/19/2020
ms.locfileid: "49720091"
---
# <a name="authenticationsourcefilter-resource-type"></a><span data-ttu-id="4442f-103">tipo de recurso authenticationSourceFilter</span><span class="sxs-lookup"><span data-stu-id="4442f-103">authenticationSourceFilter resource type</span></span>

<span data-ttu-id="4442f-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="4442f-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="4442f-105">Filtro com base na origem da autenticação que é usada para determinar se o ouvinte é avaliado.</span><span class="sxs-lookup"><span data-stu-id="4442f-105">Filter based on the source of the authentication that is used to determine whether the listener is evaluated.</span></span>

<span data-ttu-id="4442f-106">A propriedade **includeApplications** pode ser usada para habilitar a inscrição de autoatendimento em um aplicativo no Azure Active Directory.</span><span class="sxs-lookup"><span data-stu-id="4442f-106">The **includeApplications** property can be used to enable self-service sign up on an application in Azure Active Directory.</span></span> <span data-ttu-id="4442f-107">Saiba mais lendo nossa documentação para [habilitar aplicativos em um fluxo de usuário de inscrição de autoatendimento](https://docs.microsoft.com/azure/active-directory/external-identities/self-service-sign-up-user-flow#add-applications-to-the-self-service-sign-up-user-flow).</span><span class="sxs-lookup"><span data-stu-id="4442f-107">Learn more by reading our documentation for [enabling applications in a self-service sign up user flow](https://docs.microsoft.com/azure/active-directory/external-identities/self-service-sign-up-user-flow#add-applications-to-the-self-service-sign-up-user-flow).</span></span>

## <a name="properties"></a><span data-ttu-id="4442f-108">Propriedades</span><span class="sxs-lookup"><span data-stu-id="4442f-108">Properties</span></span>

|<span data-ttu-id="4442f-109">Propriedade</span><span class="sxs-lookup"><span data-stu-id="4442f-109">Property</span></span>|<span data-ttu-id="4442f-110">Tipo</span><span class="sxs-lookup"><span data-stu-id="4442f-110">Type</span></span>|<span data-ttu-id="4442f-111">Descrição</span><span class="sxs-lookup"><span data-stu-id="4442f-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="4442f-112">includeApplications</span><span class="sxs-lookup"><span data-stu-id="4442f-112">includeApplications</span></span>|<span data-ttu-id="4442f-113">Coleção de cadeias de caracteres</span><span class="sxs-lookup"><span data-stu-id="4442f-113">String collection</span></span>|<span data-ttu-id="4442f-114">Aplicativos a serem incluídos para avaliação do [authenticationListener](../resources/authenticationlistener.md).</span><span class="sxs-lookup"><span data-stu-id="4442f-114">Applications to include for evaluation of the [authenticationListener](../resources/authenticationlistener.md).</span></span> <span data-ttu-id="4442f-115">Esses aplicativos acionam a ação associada quando usados como o aplicativo cliente no fluxo de autenticação.</span><span class="sxs-lookup"><span data-stu-id="4442f-115">These applications trigger the associated action when used as the client application in the authentication flow.</span></span> <span data-ttu-id="4442f-116">O identificador de aplicativo é a ID do cliente do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="4442f-116">The application identifer is the application's client id.</span></span>|

## <a name="relationships"></a><span data-ttu-id="4442f-117">Relações</span><span class="sxs-lookup"><span data-stu-id="4442f-117">Relationships</span></span>

<span data-ttu-id="4442f-118">Nenhum</span><span class="sxs-lookup"><span data-stu-id="4442f-118">None.</span></span>

## <a name="json-representation"></a><span data-ttu-id="4442f-119">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="4442f-119">JSON representation</span></span>

<span data-ttu-id="4442f-120">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="4442f-120">The following is a JSON representation of the resource.</span></span>
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
