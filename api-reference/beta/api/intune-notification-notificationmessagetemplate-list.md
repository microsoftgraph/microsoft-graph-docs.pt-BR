---
title: Listar notificationMessageTemplates
description: Listar propriedades e relações dos objetos notificationMessageTemplate.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 0f9503fd2fdc2f155a5ed3c4810f349cfc31f933
ms.sourcegitcommit: f592c9ff96ceeb40caa67fcfe90fe6c8525cb7d2
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/23/2021
ms.locfileid: "51152821"
---
# <a name="list-notificationmessagetemplates"></a><span data-ttu-id="b95cf-103">Listar notificationMessageTemplates</span><span class="sxs-lookup"><span data-stu-id="b95cf-103">List notificationMessageTemplates</span></span>

<span data-ttu-id="b95cf-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="b95cf-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="b95cf-105">**Importante:** As APIs do Microsoft Graph na versão /beta estão sujeitas a alterações; não há suporte para uso de produção.</span><span class="sxs-lookup"><span data-stu-id="b95cf-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="b95cf-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="b95cf-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="b95cf-107">Listar propriedades e relações dos objetos [notificationMessageTemplate](../resources/intune-notification-notificationmessagetemplate.md).</span><span class="sxs-lookup"><span data-stu-id="b95cf-107">List properties and relationships of the [notificationMessageTemplate](../resources/intune-notification-notificationmessagetemplate.md) objects.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="b95cf-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="b95cf-108">Prerequisites</span></span>
<span data-ttu-id="b95cf-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="b95cf-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="b95cf-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="b95cf-111">Permission type</span></span>|<span data-ttu-id="b95cf-112">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="b95cf-112">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="b95cf-113">Delegada (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="b95cf-113">Delegated (work or school account)</span></span>|<span data-ttu-id="b95cf-114">DeviceManagementServiceConfig.Read.All, DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="b95cf-114">DeviceManagementServiceConfig.Read.All, DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="b95cf-115">Delegada (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="b95cf-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="b95cf-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="b95cf-116">Not supported.</span></span>|
|<span data-ttu-id="b95cf-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="b95cf-117">Application</span></span>|<span data-ttu-id="b95cf-118">DeviceManagementServiceConfig.Read.All, DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="b95cf-118">DeviceManagementServiceConfig.Read.All, DeviceManagementServiceConfig.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="b95cf-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="b95cf-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/notificationMessageTemplates
```

## <a name="request-headers"></a><span data-ttu-id="b95cf-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="b95cf-120">Request headers</span></span>
|<span data-ttu-id="b95cf-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="b95cf-121">Header</span></span>|<span data-ttu-id="b95cf-122">Valor</span><span class="sxs-lookup"><span data-stu-id="b95cf-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="b95cf-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="b95cf-123">Authorization</span></span>|<span data-ttu-id="b95cf-124">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="b95cf-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="b95cf-125">Aceitar</span><span class="sxs-lookup"><span data-stu-id="b95cf-125">Accept</span></span>|<span data-ttu-id="b95cf-126">application/json</span><span class="sxs-lookup"><span data-stu-id="b95cf-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="b95cf-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="b95cf-127">Request body</span></span>
<span data-ttu-id="b95cf-128">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="b95cf-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="b95cf-129">Resposta</span><span class="sxs-lookup"><span data-stu-id="b95cf-129">Response</span></span>
<span data-ttu-id="b95cf-130">Se tiver êxito, este método retornará um código de resposta `200 OK` e uma coleção de objetos [notificationMessageTemplate](../resources/intune-notification-notificationmessagetemplate.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="b95cf-130">If successful, this method returns a `200 OK` response code and a collection of [notificationMessageTemplate](../resources/intune-notification-notificationmessagetemplate.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="b95cf-131">Exemplo</span><span class="sxs-lookup"><span data-stu-id="b95cf-131">Example</span></span>

### <a name="request"></a><span data-ttu-id="b95cf-132">Solicitação</span><span class="sxs-lookup"><span data-stu-id="b95cf-132">Request</span></span>
<span data-ttu-id="b95cf-133">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="b95cf-133">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/notificationMessageTemplates
```

### <a name="response"></a><span data-ttu-id="b95cf-134">Resposta</span><span class="sxs-lookup"><span data-stu-id="b95cf-134">Response</span></span>
<span data-ttu-id="b95cf-p102">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="b95cf-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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




