---
title: Obter telecomExpenseManagementPartner
description: Ler propriedades de leitura e relações do objeto telecomExpenseManagementPartner.
author: tfitzmac
ms.openlocfilehash: 843f10270ac9713c02bf46e0634190e44323e450
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 12/18/2018
ms.locfileid: "27321599"
---
# <a name="get-telecomexpensemanagementpartner"></a><span data-ttu-id="21092-103">Obter telecomExpenseManagementPartner</span><span class="sxs-lookup"><span data-stu-id="21092-103">Get telecomExpenseManagementPartner</span></span>

> <span data-ttu-id="21092-104">**Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="21092-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="21092-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="21092-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="21092-106">**Observação:** O uso das APIs do Microsoft Graph para configurar controles e políticas do Intune ainda exige que o serviço do Intune seja [corretamente licenciado](https://go.microsoft.com/fwlink/?linkid=839381) pelo cliente.</span><span class="sxs-lookup"><span data-stu-id="21092-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="21092-107">Ler propriedades de leitura e relações do objeto [telecomExpenseManagementPartner](../resources/intune-tem-telecomexpensemanagementpartner.md).</span><span class="sxs-lookup"><span data-stu-id="21092-107">Read properties and relationships of the [telecomExpenseManagementPartner](../resources/intune-tem-telecomexpensemanagementpartner.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="21092-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="21092-108">Prerequisites</span></span>
<span data-ttu-id="21092-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="21092-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="21092-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="21092-111">Permission type</span></span>|<span data-ttu-id="21092-112">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="21092-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="21092-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="21092-113">Delegated (work or school account)</span></span>|<span data-ttu-id="21092-114">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span><span class="sxs-lookup"><span data-stu-id="21092-114">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span></span>|
|<span data-ttu-id="21092-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="21092-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="21092-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="21092-116">Not supported.</span></span>|
|<span data-ttu-id="21092-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="21092-117">Application</span></span>|<span data-ttu-id="21092-118">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="21092-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="21092-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="21092-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/telecomExpenseManagementPartners/{telecomExpenseManagementPartnerId}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="21092-120">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="21092-120">Optional query parameters</span></span>
<span data-ttu-id="21092-121">Este método dá suporte a [Parâmetros de consulta OData](https://developer.microsoft.com/graph/docs/concepts/query_parameters) para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="21092-121">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>
## <a name="request-headers"></a><span data-ttu-id="21092-122">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="21092-122">Request headers</span></span>
|<span data-ttu-id="21092-123">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="21092-123">Header</span></span>|<span data-ttu-id="21092-124">Valor</span><span class="sxs-lookup"><span data-stu-id="21092-124">Value</span></span>|
|:---|:---|
|<span data-ttu-id="21092-125">Autorização</span><span class="sxs-lookup"><span data-stu-id="21092-125">Authorization</span></span>|<span data-ttu-id="21092-126">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="21092-126">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="21092-127">Accept</span><span class="sxs-lookup"><span data-stu-id="21092-127">Accept</span></span>|<span data-ttu-id="21092-128">application/json</span><span class="sxs-lookup"><span data-stu-id="21092-128">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="21092-129">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="21092-129">Request body</span></span>
<span data-ttu-id="21092-130">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="21092-130">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="21092-131">Resposta</span><span class="sxs-lookup"><span data-stu-id="21092-131">Response</span></span>
<span data-ttu-id="21092-132">Se tiver êxito, este método retornará um código de resposta `200 OK` e um objeto [telecomExpenseManagementPartner](../resources/intune-tem-telecomexpensemanagementpartner.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="21092-132">If successful, this method returns a `200 OK` response code and [telecomExpenseManagementPartner](../resources/intune-tem-telecomexpensemanagementpartner.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="21092-133">Exemplo</span><span class="sxs-lookup"><span data-stu-id="21092-133">Example</span></span>
### <a name="request"></a><span data-ttu-id="21092-134">Solicitação</span><span class="sxs-lookup"><span data-stu-id="21092-134">Request</span></span>
<span data-ttu-id="21092-135">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="21092-135">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/telecomExpenseManagementPartners/{telecomExpenseManagementPartnerId}
```

### <a name="response"></a><span data-ttu-id="21092-136">Resposta</span><span class="sxs-lookup"><span data-stu-id="21092-136">Response</span></span>
<span data-ttu-id="21092-p103">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="21092-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 330

{
  "value": {
    "@odata.type": "#microsoft.graph.telecomExpenseManagementPartner",
    "id": "47a3b399-b399-47a3-99b3-a34799b3a347",
    "displayName": "Display Name value",
    "url": "Url value",
    "appAuthorized": true,
    "enabled": true,
    "lastConnectionDateTime": "2016-12-31T23:58:36.6670033-08:00"
  }
}
```





