---
title: Listar notificationMessageTemplates
description: Listar propriedades e relações dos objetos notificationMessageTemplate.
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 12e7bc9ce4b3d2cae3df0d69834981f90c65ef73
ms.sourcegitcommit: 86903a4730bbd825eabb7f0a1b2429723cc8b1e6
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/26/2019
ms.locfileid: "37191079"
---
# <a name="list-notificationmessagetemplates"></a><span data-ttu-id="1e403-103">Listar notificationMessageTemplates</span><span class="sxs-lookup"><span data-stu-id="1e403-103">List notificationMessageTemplates</span></span>

> <span data-ttu-id="1e403-104">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="1e403-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="1e403-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="1e403-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="1e403-106">Listar propriedades e relações dos objetos [notificationMessageTemplate](../resources/intune-notification-notificationmessagetemplate.md).</span><span class="sxs-lookup"><span data-stu-id="1e403-106">List properties and relationships of the [notificationMessageTemplate](../resources/intune-notification-notificationmessagetemplate.md) objects.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="1e403-107">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="1e403-107">Prerequisites</span></span>
<span data-ttu-id="1e403-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="1e403-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="1e403-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="1e403-110">Permission type</span></span>|<span data-ttu-id="1e403-111">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="1e403-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="1e403-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="1e403-112">Delegated (work or school account)</span></span>|<span data-ttu-id="1e403-113">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span><span class="sxs-lookup"><span data-stu-id="1e403-113">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span></span>|
|<span data-ttu-id="1e403-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="1e403-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="1e403-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="1e403-115">Not supported.</span></span>|
|<span data-ttu-id="1e403-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="1e403-116">Application</span></span>|<span data-ttu-id="1e403-117">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span><span class="sxs-lookup"><span data-stu-id="1e403-117">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="1e403-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="1e403-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/notificationMessageTemplates
```

## <a name="request-headers"></a><span data-ttu-id="1e403-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="1e403-119">Request headers</span></span>
|<span data-ttu-id="1e403-120">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="1e403-120">Header</span></span>|<span data-ttu-id="1e403-121">Valor</span><span class="sxs-lookup"><span data-stu-id="1e403-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="1e403-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="1e403-122">Authorization</span></span>|<span data-ttu-id="1e403-123">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="1e403-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="1e403-124">Aceitar</span><span class="sxs-lookup"><span data-stu-id="1e403-124">Accept</span></span>|<span data-ttu-id="1e403-125">application/json</span><span class="sxs-lookup"><span data-stu-id="1e403-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="1e403-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="1e403-126">Request body</span></span>
<span data-ttu-id="1e403-127">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="1e403-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="1e403-128">Resposta</span><span class="sxs-lookup"><span data-stu-id="1e403-128">Response</span></span>
<span data-ttu-id="1e403-129">Se tiver êxito, este método retornará um código de resposta `200 OK` e uma coleção de objetos [notificationMessageTemplate](../resources/intune-notification-notificationmessagetemplate.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="1e403-129">If successful, this method returns a `200 OK` response code and a collection of [notificationMessageTemplate](../resources/intune-notification-notificationmessagetemplate.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="1e403-130">Exemplo</span><span class="sxs-lookup"><span data-stu-id="1e403-130">Example</span></span>

### <a name="request"></a><span data-ttu-id="1e403-131">Solicitação</span><span class="sxs-lookup"><span data-stu-id="1e403-131">Request</span></span>
<span data-ttu-id="1e403-132">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="1e403-132">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/notificationMessageTemplates
```

### <a name="response"></a><span data-ttu-id="1e403-133">Resposta</span><span class="sxs-lookup"><span data-stu-id="1e403-133">Response</span></span>
<span data-ttu-id="1e403-p102">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="1e403-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 441

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.notificationMessageTemplate",
      "id": "e1db399b-399b-e1db-9b39-dbe19b39dbe1",
      "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
      "displayName": "Display Name value",
      "defaultLocale": "Default Locale value",
      "brandingOptions": "includeCompanyLogo",
      "roleScopeTagIds": [
        "Role Scope Tag Ids value"
      ]
    }
  ]
}
```




