---
title: Get notificationMessageTemplate
description: Ler propriedades e relações do objeto notificationMessageTemplate.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: de0d8a2c3d1a802ea4f3f42936b2bfded4c03128
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/24/2019
ms.locfileid: "32561723"
---
# <a name="get-notificationmessagetemplate"></a><span data-ttu-id="0f3fc-103">Get notificationMessageTemplate</span><span class="sxs-lookup"><span data-stu-id="0f3fc-103">Get notificationMessageTemplate</span></span>

> <span data-ttu-id="0f3fc-104">**Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="0f3fc-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="0f3fc-105">Ler propriedades e relações do objeto [notificationMessageTemplate](../resources/intune-notification-notificationmessagetemplate.md).</span><span class="sxs-lookup"><span data-stu-id="0f3fc-105">Read properties and relationships of the [notificationMessageTemplate](../resources/intune-notification-notificationmessagetemplate.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="0f3fc-106">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="0f3fc-106">Prerequisites</span></span>
<span data-ttu-id="0f3fc-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="0f3fc-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="0f3fc-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="0f3fc-109">Permission type</span></span>|<span data-ttu-id="0f3fc-110">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="0f3fc-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="0f3fc-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="0f3fc-111">Delegated (work or school account)</span></span>|<span data-ttu-id="0f3fc-112">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span><span class="sxs-lookup"><span data-stu-id="0f3fc-112">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span></span>|
|<span data-ttu-id="0f3fc-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="0f3fc-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="0f3fc-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="0f3fc-114">Not supported.</span></span>|
|<span data-ttu-id="0f3fc-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="0f3fc-115">Application</span></span>|<span data-ttu-id="0f3fc-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="0f3fc-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="0f3fc-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="0f3fc-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/notificationMessageTemplates/{notificationMessageTemplateId}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="0f3fc-118">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="0f3fc-118">Optional query parameters</span></span>
<span data-ttu-id="0f3fc-119">Este método dá suporte a [Parâmetros de consulta OData](https://docs.microsoft.com/en-us/graph/query-parameters) para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="0f3fc-119">This method supports the [OData Query Parameters](https://docs.microsoft.com/en-us/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="0f3fc-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="0f3fc-120">Request headers</span></span>
|<span data-ttu-id="0f3fc-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="0f3fc-121">Header</span></span>|<span data-ttu-id="0f3fc-122">Valor</span><span class="sxs-lookup"><span data-stu-id="0f3fc-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="0f3fc-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="0f3fc-123">Authorization</span></span>|<span data-ttu-id="0f3fc-124">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="0f3fc-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="0f3fc-125">Aceitar</span><span class="sxs-lookup"><span data-stu-id="0f3fc-125">Accept</span></span>|<span data-ttu-id="0f3fc-126">application/json</span><span class="sxs-lookup"><span data-stu-id="0f3fc-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="0f3fc-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="0f3fc-127">Request body</span></span>
<span data-ttu-id="0f3fc-128">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="0f3fc-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="0f3fc-129">Resposta</span><span class="sxs-lookup"><span data-stu-id="0f3fc-129">Response</span></span>
<span data-ttu-id="0f3fc-130">Se bem-sucedido, este método retornará um código de resposta `200 OK` e um objeto [notificationMessageTemplate](../resources/intune-notification-notificationmessagetemplate.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="0f3fc-130">If successful, this method returns a `200 OK` response code and [notificationMessageTemplate](../resources/intune-notification-notificationmessagetemplate.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="0f3fc-131">Exemplo</span><span class="sxs-lookup"><span data-stu-id="0f3fc-131">Example</span></span>

### <a name="request"></a><span data-ttu-id="0f3fc-132">Solicitação</span><span class="sxs-lookup"><span data-stu-id="0f3fc-132">Request</span></span>
<span data-ttu-id="0f3fc-133">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="0f3fc-133">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/v1.0/deviceManagement/notificationMessageTemplates/{notificationMessageTemplateId}
```

### <a name="response"></a><span data-ttu-id="0f3fc-134">Resposta</span><span class="sxs-lookup"><span data-stu-id="0f3fc-134">Response</span></span>
<span data-ttu-id="0f3fc-p102">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="0f3fc-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 341

{
  "value": {
    "@odata.type": "#microsoft.graph.notificationMessageTemplate",
    "id": "e1db399b-399b-e1db-9b39-dbe19b39dbe1",
    "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
    "displayName": "Display Name value",
    "defaultLocale": "Default Locale value",
    "brandingOptions": "includeCompanyLogo"
  }
}
```



