---
title: Tipo de recurso signInActivity
description: Fornece a última data de assinatura para um usuário específico.
localization_priority: Normal
author: besiler
ms.prod: identity-and-access-reports
doc_type: resourcePageType
ms.openlocfilehash: 7d57324b7953b865b98c01d6b16236dea54e73a5
ms.sourcegitcommit: 9d98d9e9cc1e193850ab9b82aaaf906d70e1378b
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/12/2021
ms.locfileid: "50761055"
---
# <a name="signinactivity-resource-type"></a><span data-ttu-id="7dd4c-103">Tipo de recurso signInActivity</span><span class="sxs-lookup"><span data-stu-id="7dd4c-103">signInActivity resource type</span></span>

<span data-ttu-id="7dd4c-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="7dd4c-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="7dd4c-105">Fornece a última data de assinatura para um usuário [específico.](user.md)</span><span class="sxs-lookup"><span data-stu-id="7dd4c-105">Provides the last signed-in date for a specific [user](user.md).</span></span>

## <a name="properties"></a><span data-ttu-id="7dd4c-106">Propriedades</span><span class="sxs-lookup"><span data-stu-id="7dd4c-106">Properties</span></span>

| <span data-ttu-id="7dd4c-107">Propriedade</span><span class="sxs-lookup"><span data-stu-id="7dd4c-107">Property</span></span>     | <span data-ttu-id="7dd4c-108">Tipo</span><span class="sxs-lookup"><span data-stu-id="7dd4c-108">Type</span></span>        | <span data-ttu-id="7dd4c-109">Descrição</span><span class="sxs-lookup"><span data-stu-id="7dd4c-109">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="7dd4c-110">lastSignInDateTime</span><span class="sxs-lookup"><span data-stu-id="7dd4c-110">lastSignInDateTime</span></span>|<span data-ttu-id="7dd4c-111">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="7dd4c-111">DateTimeOffset</span></span>|<span data-ttu-id="7dd4c-112">A última data de login interativa para um usuário específico.</span><span class="sxs-lookup"><span data-stu-id="7dd4c-112">The last interactive sign-in date for a specific user.</span></span> <span data-ttu-id="7dd4c-113">Você pode usar esse campo para calcular a última vez que um usuário se inscreveu no diretório com um método de autenticação interativa.</span><span class="sxs-lookup"><span data-stu-id="7dd4c-113">You can use this field to calculate the last time a user signed in to the directory with an interactive authentication method.</span></span> <span data-ttu-id="7dd4c-114">Esse campo pode ser usado para criar relatórios, como usuários inativos.</span><span class="sxs-lookup"><span data-stu-id="7dd4c-114">This field can be used to build reports, such as inactive users.</span></span> <span data-ttu-id="7dd4c-115">O carimbo de data/hora representa informações de data e hora usando o formato ISO 8601 e está sempre no horário UTC.</span><span class="sxs-lookup"><span data-stu-id="7dd4c-115">The timestamp represents date and time information using ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="7dd4c-116">Por exemplo, meia-noite UTC em 1º de janeiro de 2014 é: `'2014-01-01T00:00:00Z'` .</span><span class="sxs-lookup"><span data-stu-id="7dd4c-116">For example, midnight UTC on Jan 1, 2014 is: `'2014-01-01T00:00:00Z'`.</span></span> <span data-ttu-id="7dd4c-117">Para obter mais informações sobre como usar o valor dessa propriedade, consulte Gerenciar contas de usuário [inativas no Azure AD](/azure/active-directory/reports-monitoring/howto-manage-inactive-user-accounts).</span><span class="sxs-lookup"><span data-stu-id="7dd4c-117">For more information about using the value of this property, see [Manage inactive user accounts in Azure AD](/azure/active-directory/reports-monitoring/howto-manage-inactive-user-accounts).</span></span>|
|<span data-ttu-id="7dd4c-118">lastSignInRequestId</span><span class="sxs-lookup"><span data-stu-id="7dd4c-118">lastSignInRequestId</span></span>|<span data-ttu-id="7dd4c-119">Cadeia de Caracteres</span><span class="sxs-lookup"><span data-stu-id="7dd4c-119">String</span></span>|<span data-ttu-id="7dd4c-120">ID de solicitação do último login executado por esse usuário.</span><span class="sxs-lookup"><span data-stu-id="7dd4c-120">Request ID of the last sign-in performed by this user.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="7dd4c-121">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="7dd4c-121">JSON representation</span></span>

<span data-ttu-id="7dd4c-122">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="7dd4c-122">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.signInActivity",
  "baseType": null
}-->

```json
{
  "lastSignInDateTime": "String (timestamp)",
  "lastSignInRequestId": "String"
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "signInActivity resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
