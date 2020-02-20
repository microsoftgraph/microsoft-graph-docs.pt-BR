---
title: Listar termsAndConditionsAcceptanceStatuses
description: Listar propriedades e relações dos objetos termsAndConditionsAcceptanceStatus.
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: d413321fedbdb3d7380156f99386235c3d74e27c
ms.sourcegitcommit: 5cf98ba275547e5659df4af1eeeff0ba484b0e67
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 02/20/2020
ms.locfileid: "42160281"
---
# <a name="list-termsandconditionsacceptancestatuses"></a><span data-ttu-id="ef8f8-103">Listar termsAndConditionsAcceptanceStatuses</span><span class="sxs-lookup"><span data-stu-id="ef8f8-103">List termsAndConditionsAcceptanceStatuses</span></span>

> <span data-ttu-id="ef8f8-104">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="ef8f8-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="ef8f8-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="ef8f8-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="ef8f8-106">Listar propriedades e relações dos objetos [termsAndConditionsAcceptanceStatus](../resources/intune-companyterms-termsandconditionsacceptancestatus.md).</span><span class="sxs-lookup"><span data-stu-id="ef8f8-106">List properties and relationships of the [termsAndConditionsAcceptanceStatus](../resources/intune-companyterms-termsandconditionsacceptancestatus.md) objects.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="ef8f8-107">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="ef8f8-107">Prerequisites</span></span>
<span data-ttu-id="ef8f8-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="ef8f8-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="ef8f8-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="ef8f8-110">Permission type</span></span>|<span data-ttu-id="ef8f8-111">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="ef8f8-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="ef8f8-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="ef8f8-112">Delegated (work or school account)</span></span>|<span data-ttu-id="ef8f8-113">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span><span class="sxs-lookup"><span data-stu-id="ef8f8-113">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span></span>|
|<span data-ttu-id="ef8f8-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="ef8f8-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="ef8f8-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="ef8f8-115">Not supported.</span></span>|
|<span data-ttu-id="ef8f8-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="ef8f8-116">Application</span></span>|<span data-ttu-id="ef8f8-117">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span><span class="sxs-lookup"><span data-stu-id="ef8f8-117">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="ef8f8-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="ef8f8-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/termsAndConditions/{termsAndConditionsId}/acceptanceStatuses
```

## <a name="request-headers"></a><span data-ttu-id="ef8f8-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="ef8f8-119">Request headers</span></span>
|<span data-ttu-id="ef8f8-120">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="ef8f8-120">Header</span></span>|<span data-ttu-id="ef8f8-121">Valor</span><span class="sxs-lookup"><span data-stu-id="ef8f8-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="ef8f8-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="ef8f8-122">Authorization</span></span>|<span data-ttu-id="ef8f8-123">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="ef8f8-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="ef8f8-124">Aceitar</span><span class="sxs-lookup"><span data-stu-id="ef8f8-124">Accept</span></span>|<span data-ttu-id="ef8f8-125">application/json</span><span class="sxs-lookup"><span data-stu-id="ef8f8-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="ef8f8-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="ef8f8-126">Request body</span></span>
<span data-ttu-id="ef8f8-127">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="ef8f8-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="ef8f8-128">Resposta</span><span class="sxs-lookup"><span data-stu-id="ef8f8-128">Response</span></span>
<span data-ttu-id="ef8f8-129">Se tiver êxito, este método retornará um código de resposta `200 OK` e uma coleção de objetos [termsAndConditionsAcceptanceStatus](../resources/intune-companyterms-termsandconditionsacceptancestatus.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="ef8f8-129">If successful, this method returns a `200 OK` response code and a collection of [termsAndConditionsAcceptanceStatus](../resources/intune-companyterms-termsandconditionsacceptancestatus.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="ef8f8-130">Exemplo</span><span class="sxs-lookup"><span data-stu-id="ef8f8-130">Example</span></span>

### <a name="request"></a><span data-ttu-id="ef8f8-131">Solicitação</span><span class="sxs-lookup"><span data-stu-id="ef8f8-131">Request</span></span>
<span data-ttu-id="ef8f8-132">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="ef8f8-132">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/termsAndConditions/{termsAndConditionsId}/acceptanceStatuses
```

### <a name="response"></a><span data-ttu-id="ef8f8-133">Resposta</span><span class="sxs-lookup"><span data-stu-id="ef8f8-133">Response</span></span>
<span data-ttu-id="ef8f8-p102">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="ef8f8-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 370

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.termsAndConditionsAcceptanceStatus",
      "id": "a045ce1a-ce1a-a045-1ace-45a01ace45a0",
      "userDisplayName": "User Display Name value",
      "acceptedVersion": 15,
      "acceptedDateTime": "2016-12-31T23:57:43.6165506-08:00",
      "userPrincipalName": "User Principal Name value"
    }
  ]
}
```





