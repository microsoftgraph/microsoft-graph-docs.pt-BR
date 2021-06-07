---
title: Listar notificationMessageTemplates
description: Listar propriedades e relações dos objetos notificationMessageTemplate.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: d878278149393e4e183df733ec3b1645dc77722f
ms.sourcegitcommit: 13f474d3e71d32a5dfe2efebb351e3a1a5aa9685
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/04/2021
ms.locfileid: "52754850"
---
# <a name="list-notificationmessagetemplates"></a><span data-ttu-id="d083a-103">Listar notificationMessageTemplates</span><span class="sxs-lookup"><span data-stu-id="d083a-103">List notificationMessageTemplates</span></span>

<span data-ttu-id="d083a-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="d083a-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="d083a-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="d083a-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="d083a-106">Listar propriedades e relações dos objetos [notificationMessageTemplate](../resources/intune-notification-notificationmessagetemplate.md).</span><span class="sxs-lookup"><span data-stu-id="d083a-106">List properties and relationships of the [notificationMessageTemplate](../resources/intune-notification-notificationmessagetemplate.md) objects.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="d083a-107">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="d083a-107">Prerequisites</span></span>
<span data-ttu-id="d083a-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="d083a-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="d083a-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="d083a-110">Permission type</span></span>|<span data-ttu-id="d083a-111">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="d083a-111">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="d083a-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="d083a-112">Delegated (work or school account)</span></span>|<span data-ttu-id="d083a-113">DeviceManagementServiceConfig.Read.All, DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="d083a-113">DeviceManagementServiceConfig.Read.All, DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="d083a-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="d083a-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="d083a-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="d083a-115">Not supported.</span></span>|
|<span data-ttu-id="d083a-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="d083a-116">Application</span></span>|<span data-ttu-id="d083a-117">DeviceManagementServiceConfig.Read.All, DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="d083a-117">DeviceManagementServiceConfig.Read.All, DeviceManagementServiceConfig.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="d083a-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="d083a-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/notificationMessageTemplates
```

## <a name="request-headers"></a><span data-ttu-id="d083a-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="d083a-119">Request headers</span></span>
|<span data-ttu-id="d083a-120">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="d083a-120">Header</span></span>|<span data-ttu-id="d083a-121">Valor</span><span class="sxs-lookup"><span data-stu-id="d083a-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="d083a-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="d083a-122">Authorization</span></span>|<span data-ttu-id="d083a-123">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="d083a-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="d083a-124">Aceitar</span><span class="sxs-lookup"><span data-stu-id="d083a-124">Accept</span></span>|<span data-ttu-id="d083a-125">application/json</span><span class="sxs-lookup"><span data-stu-id="d083a-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="d083a-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="d083a-126">Request body</span></span>
<span data-ttu-id="d083a-127">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="d083a-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="d083a-128">Resposta</span><span class="sxs-lookup"><span data-stu-id="d083a-128">Response</span></span>
<span data-ttu-id="d083a-129">Se tiver êxito, este método retornará um código de resposta `200 OK` e uma coleção de objetos [notificationMessageTemplate](../resources/intune-notification-notificationmessagetemplate.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="d083a-129">If successful, this method returns a `200 OK` response code and a collection of [notificationMessageTemplate](../resources/intune-notification-notificationmessagetemplate.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="d083a-130">Exemplo</span><span class="sxs-lookup"><span data-stu-id="d083a-130">Example</span></span>

### <a name="request"></a><span data-ttu-id="d083a-131">Solicitação</span><span class="sxs-lookup"><span data-stu-id="d083a-131">Request</span></span>
<span data-ttu-id="d083a-132">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="d083a-132">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/v1.0/deviceManagement/notificationMessageTemplates
```

### <a name="response"></a><span data-ttu-id="d083a-133">Resposta</span><span class="sxs-lookup"><span data-stu-id="d083a-133">Response</span></span>
<span data-ttu-id="d083a-p102">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="d083a-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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




