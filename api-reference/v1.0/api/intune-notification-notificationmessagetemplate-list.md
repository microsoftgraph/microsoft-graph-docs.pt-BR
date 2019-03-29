---
title: Listar notificationMessageTemplates
description: Listar propriedades e relações dos objetos notificationMessageTemplate.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 1334ae2925fe0d8dddc1f50a6e26b79ea6a4927e
ms.sourcegitcommit: 7b98b61db7cdbaff037e1b222ac58eef4c5bee89
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/29/2019
ms.locfileid: "30959856"
---
# <a name="list-notificationmessagetemplates"></a><span data-ttu-id="32f22-103">Listar notificationMessageTemplates</span><span class="sxs-lookup"><span data-stu-id="32f22-103">List notificationMessageTemplates</span></span>

> <span data-ttu-id="32f22-104">**Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="32f22-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="32f22-105">Listar propriedades e relações dos objetos [notificationMessageTemplate](../resources/intune-notification-notificationmessagetemplate.md).</span><span class="sxs-lookup"><span data-stu-id="32f22-105">List properties and relationships of the [notificationMessageTemplate](../resources/intune-notification-notificationmessagetemplate.md) objects.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="32f22-106">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="32f22-106">Prerequisites</span></span>
<span data-ttu-id="32f22-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="32f22-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="32f22-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="32f22-109">Permission type</span></span>|<span data-ttu-id="32f22-110">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="32f22-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="32f22-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="32f22-111">Delegated (work or school account)</span></span>|<span data-ttu-id="32f22-112">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span><span class="sxs-lookup"><span data-stu-id="32f22-112">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span></span>|
|<span data-ttu-id="32f22-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="32f22-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="32f22-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="32f22-114">Not supported.</span></span>|
|<span data-ttu-id="32f22-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="32f22-115">Application</span></span>|<span data-ttu-id="32f22-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="32f22-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="32f22-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="32f22-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/notificationMessageTemplates
```

## <a name="request-headers"></a><span data-ttu-id="32f22-118">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="32f22-118">Request headers</span></span>
|<span data-ttu-id="32f22-119">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="32f22-119">Header</span></span>|<span data-ttu-id="32f22-120">Valor</span><span class="sxs-lookup"><span data-stu-id="32f22-120">Value</span></span>|
|:---|:---|
|<span data-ttu-id="32f22-121">Autorização</span><span class="sxs-lookup"><span data-stu-id="32f22-121">Authorization</span></span>|<span data-ttu-id="32f22-122">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="32f22-122">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="32f22-123">Aceitar</span><span class="sxs-lookup"><span data-stu-id="32f22-123">Accept</span></span>|<span data-ttu-id="32f22-124">application/json</span><span class="sxs-lookup"><span data-stu-id="32f22-124">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="32f22-125">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="32f22-125">Request body</span></span>
<span data-ttu-id="32f22-126">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="32f22-126">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="32f22-127">Resposta</span><span class="sxs-lookup"><span data-stu-id="32f22-127">Response</span></span>
<span data-ttu-id="32f22-128">Se tiver êxito, este método retornará um código de resposta `200 OK` e uma coleção de objetos [notificationMessageTemplate](../resources/intune-notification-notificationmessagetemplate.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="32f22-128">If successful, this method returns a `200 OK` response code and a collection of [notificationMessageTemplate](../resources/intune-notification-notificationmessagetemplate.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="32f22-129">Exemplo</span><span class="sxs-lookup"><span data-stu-id="32f22-129">Example</span></span>

### <a name="request"></a><span data-ttu-id="32f22-130">Solicitação</span><span class="sxs-lookup"><span data-stu-id="32f22-130">Request</span></span>
<span data-ttu-id="32f22-131">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="32f22-131">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/v1.0/deviceManagement/notificationMessageTemplates
```

### <a name="response"></a><span data-ttu-id="32f22-132">Resposta</span><span class="sxs-lookup"><span data-stu-id="32f22-132">Response</span></span>
<span data-ttu-id="32f22-p102">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="32f22-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 367

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.notificationMessageTemplate",
      "id": "e1db399b-399b-e1db-9b39-dbe19b39dbe1",
      "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
      "displayName": "Display Name value",
      "defaultLocale": "Default Locale value",
      "brandingOptions": "includeCompanyLogo"
    }
  ]
}
```



