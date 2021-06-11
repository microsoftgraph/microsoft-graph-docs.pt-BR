---
title: Tipo de recurso accessReviewNotificationRecipientItem
description: Define usuários ou grupos que receberão notificações de acesso a notificações de revisão.
author: isabelleatmsft
localization_priority: Normal
ms.prod: governance
doc_type: resourcePageType
ms.openlocfilehash: 3d6ed767f1350f3e4a43a1b31363920ffb58a9b5
ms.sourcegitcommit: 7abb0672a38a6d9b11a2e0d2cc221222cb8358bb
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/11/2021
ms.locfileid: "52896729"
---
# <a name="accessreviewnotificationrecipientitem-resource-type"></a><span data-ttu-id="0b716-103">Tipo de recurso accessReviewNotificationRecipientItem</span><span class="sxs-lookup"><span data-stu-id="0b716-103">accessReviewNotificationRecipientItem resource type</span></span>

<span data-ttu-id="0b716-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="0b716-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

[!INCLUDE [accessreviews-disclaimer-v2](../../includes/accessreviews-disclaimer-v2.md)]


<span data-ttu-id="0b716-105">Representa um evento de notificação de revisão [de](accessreviewsv2-root.md) acesso do Azure AD em uma instância de uma revisão.</span><span class="sxs-lookup"><span data-stu-id="0b716-105">Represents an Azure AD [access review](accessreviewsv2-root.md) notification event on an instance of a review.</span></span> <span data-ttu-id="0b716-106">Este item contém um tipo de modelo de email e propriedades de destinatário para habilitar o envio de determinado tipo de notificações para uma determinada instância de revisão [de acesso.](accessreviewinstance.md)</span><span class="sxs-lookup"><span data-stu-id="0b716-106">This item contains an email template type and recipient properties to enable sending certain type of notifications for a given [access review instance](accessreviewinstance.md).</span></span>

## <a name="properties"></a><span data-ttu-id="0b716-107">Propriedades</span><span class="sxs-lookup"><span data-stu-id="0b716-107">Properties</span></span>

| <span data-ttu-id="0b716-108">Propriedade</span><span class="sxs-lookup"><span data-stu-id="0b716-108">Property</span></span>                     | <span data-ttu-id="0b716-109">Tipo</span><span class="sxs-lookup"><span data-stu-id="0b716-109">Type</span></span>     | <span data-ttu-id="0b716-110">Descrição</span><span class="sxs-lookup"><span data-stu-id="0b716-110">Description</span></span>                          |
| :--------------------------- | :------  | :----------                          |
| <span data-ttu-id="0b716-111">notificationTemplateType</span><span class="sxs-lookup"><span data-stu-id="0b716-111">notificationTemplateType</span></span>  |<span data-ttu-id="0b716-112">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="0b716-112">String</span></span>  | <span data-ttu-id="0b716-113">Indica o tipo de email de revisão de acesso a ser enviado.</span><span class="sxs-lookup"><span data-stu-id="0b716-113">Indicates the type of access review email to be sent.</span></span> <span data-ttu-id="0b716-114">O tipo de modelo com suporte é o que envia notificações de conclusão `CompletedAdditionalRecipients` de revisão aos destinatários.</span><span class="sxs-lookup"><span data-stu-id="0b716-114">Supported template type is `CompletedAdditionalRecipients` which sends review completion notifications to the recipients.</span></span>|
| <span data-ttu-id="0b716-115">notificationRecipientScope</span><span class="sxs-lookup"><span data-stu-id="0b716-115">notificationRecipientScope</span></span> |[<span data-ttu-id="0b716-116">accessReviewNotificationRecipientScope</span><span class="sxs-lookup"><span data-stu-id="0b716-116">accessReviewNotificationRecipientScope</span></span>](../resources/accessreviewnotificationrecipientscope.md)  | <span data-ttu-id="0b716-117">Determina o destinatário do email de notificação.</span><span class="sxs-lookup"><span data-stu-id="0b716-117">Determines the recipient of the notification email.</span></span>|

## <a name="relationships"></a><span data-ttu-id="0b716-118">Relações</span><span class="sxs-lookup"><span data-stu-id="0b716-118">Relationships</span></span>
<span data-ttu-id="0b716-119">Nenhum</span><span class="sxs-lookup"><span data-stu-id="0b716-119">None.</span></span>


## <a name="json-representation"></a><span data-ttu-id="0b716-120">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="0b716-120">JSON representation</span></span>

<span data-ttu-id="0b716-121">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="0b716-121">Here is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.accessReviewNotificationRecipientItem",
  "openType": true
}
-->

```json
{
  "@odata.type":"#microsoft.graph.accessReviewNotificationRecipientItem",
  "notificationRecipientScope": {
      "@odata.type":"#microsoft.graph.accessReviewNotificationRecipientQueryScope"                
    },
  "notificationTemplateType": "String"
}
```
