---
title: Get userInstallStateSummary
description: Ler propriedades e relações do objeto userInstallStateSummary.
author: tfitzmac
ms.openlocfilehash: 152160f99220f95c9f743ee637da35c693400d41
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 12/18/2018
ms.locfileid: "27358342"
---
# <a name="get-userinstallstatesummary"></a><span data-ttu-id="fafaf-103">Get userInstallStateSummary</span><span class="sxs-lookup"><span data-stu-id="fafaf-103">Get userInstallStateSummary</span></span>

> <span data-ttu-id="fafaf-104">**Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="fafaf-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="fafaf-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="fafaf-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="fafaf-106">**Observação:** O uso das APIs do Microsoft Graph para configurar controles e políticas do Intune ainda exige que o serviço do Intune seja [corretamente licenciado](https://go.microsoft.com/fwlink/?linkid=839381) pelo cliente.</span><span class="sxs-lookup"><span data-stu-id="fafaf-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="fafaf-107">Ler propriedades e relações do objeto [userInstallStateSummary](../resources/intune-books-userinstallstatesummary.md).</span><span class="sxs-lookup"><span data-stu-id="fafaf-107">Read properties and relationships of the [userInstallStateSummary](../resources/intune-books-userinstallstatesummary.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="fafaf-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="fafaf-108">Prerequisites</span></span>
<span data-ttu-id="fafaf-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="fafaf-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="fafaf-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="fafaf-111">Permission type</span></span>|<span data-ttu-id="fafaf-112">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="fafaf-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="fafaf-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="fafaf-113">Delegated (work or school account)</span></span>|<span data-ttu-id="fafaf-114">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span><span class="sxs-lookup"><span data-stu-id="fafaf-114">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span></span>|
|<span data-ttu-id="fafaf-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="fafaf-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="fafaf-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="fafaf-116">Not supported.</span></span>|
|<span data-ttu-id="fafaf-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="fafaf-117">Application</span></span>|<span data-ttu-id="fafaf-118">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="fafaf-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="fafaf-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="fafaf-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceAppManagement/managedEBooks/{managedEBookId}/userStateSummary/{userInstallStateSummaryId}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="fafaf-120">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="fafaf-120">Optional query parameters</span></span>
<span data-ttu-id="fafaf-121">Este método dá suporte a [Parâmetros de consulta OData](https://developer.microsoft.com/graph/docs/concepts/query_parameters) para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="fafaf-121">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>
## <a name="request-headers"></a><span data-ttu-id="fafaf-122">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="fafaf-122">Request headers</span></span>
|<span data-ttu-id="fafaf-123">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="fafaf-123">Header</span></span>|<span data-ttu-id="fafaf-124">Valor</span><span class="sxs-lookup"><span data-stu-id="fafaf-124">Value</span></span>|
|:---|:---|
|<span data-ttu-id="fafaf-125">Autorização</span><span class="sxs-lookup"><span data-stu-id="fafaf-125">Authorization</span></span>|<span data-ttu-id="fafaf-126">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="fafaf-126">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="fafaf-127">Accept</span><span class="sxs-lookup"><span data-stu-id="fafaf-127">Accept</span></span>|<span data-ttu-id="fafaf-128">application/json</span><span class="sxs-lookup"><span data-stu-id="fafaf-128">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="fafaf-129">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="fafaf-129">Request body</span></span>
<span data-ttu-id="fafaf-130">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="fafaf-130">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="fafaf-131">Resposta</span><span class="sxs-lookup"><span data-stu-id="fafaf-131">Response</span></span>
<span data-ttu-id="fafaf-132">Se bem-sucedido, este método retornará um código de resposta `200 OK` e um objeto [userInstallStateSummary](../resources/intune-books-userinstallstatesummary.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="fafaf-132">If successful, this method returns a `200 OK` response code and [userInstallStateSummary](../resources/intune-books-userinstallstatesummary.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="fafaf-133">Exemplo</span><span class="sxs-lookup"><span data-stu-id="fafaf-133">Example</span></span>
### <a name="request"></a><span data-ttu-id="fafaf-134">Solicitação</span><span class="sxs-lookup"><span data-stu-id="fafaf-134">Request</span></span>
<span data-ttu-id="fafaf-135">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="fafaf-135">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceAppManagement/managedEBooks/{managedEBookId}/userStateSummary/{userInstallStateSummaryId}
```

### <a name="response"></a><span data-ttu-id="fafaf-136">Resposta</span><span class="sxs-lookup"><span data-stu-id="fafaf-136">Response</span></span>
<span data-ttu-id="fafaf-p103">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="fafaf-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 269

{
  "value": {
    "@odata.type": "#microsoft.graph.userInstallStateSummary",
    "id": "1e5b41ba-41ba-1e5b-ba41-5b1eba415b1e",
    "userName": "User Name value",
    "installedDeviceCount": 4,
    "failedDeviceCount": 1,
    "notInstalledDeviceCount": 7
  }
}
```





