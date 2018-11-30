---
title: Criar termsAndConditionsAcceptanceStatus
description: Cria um novo objeto termsAndConditionsAcceptanceStatus.
ms.openlocfilehash: 0c23689addf5c1c7a53f2d9f5a7c5f09918fd9f7
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/29/2018
ms.locfileid: "27036483"
---
# <a name="create-termsandconditionsacceptancestatus"></a><span data-ttu-id="1dcbf-103">Criar termsAndConditionsAcceptanceStatus</span><span class="sxs-lookup"><span data-stu-id="1dcbf-103">Create termsAndConditionsAcceptanceStatus</span></span>

> <span data-ttu-id="1dcbf-104">**Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="1dcbf-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="1dcbf-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="1dcbf-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="1dcbf-106">**Observação:** O uso das APIs do Microsoft Graph para configurar controles e políticas do Intune ainda exige que o serviço do Intune seja [corretamente licenciado](https://go.microsoft.com/fwlink/?linkid=839381) pelo cliente.</span><span class="sxs-lookup"><span data-stu-id="1dcbf-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="1dcbf-107">Cria um novo objeto [termsAndConditionsAcceptanceStatus](../resources/intune-companyterms-termsandconditionsacceptancestatus.md).</span><span class="sxs-lookup"><span data-stu-id="1dcbf-107">Create a new [termsAndConditionsAcceptanceStatus](../resources/intune-companyterms-termsandconditionsacceptancestatus.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="1dcbf-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="1dcbf-108">Prerequisites</span></span>
<span data-ttu-id="1dcbf-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="1dcbf-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="1dcbf-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="1dcbf-111">Permission type</span></span>|<span data-ttu-id="1dcbf-112">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="1dcbf-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="1dcbf-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="1dcbf-113">Delegated (work or school account)</span></span>|<span data-ttu-id="1dcbf-114">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="1dcbf-114">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="1dcbf-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="1dcbf-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="1dcbf-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="1dcbf-116">Not supported.</span></span>|
|<span data-ttu-id="1dcbf-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="1dcbf-117">Application</span></span>|<span data-ttu-id="1dcbf-118">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="1dcbf-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="1dcbf-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="1dcbf-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/termsAndConditions/{termsAndConditionsId}/acceptanceStatuses
```

## <a name="request-headers"></a><span data-ttu-id="1dcbf-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="1dcbf-120">Request headers</span></span>
|<span data-ttu-id="1dcbf-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="1dcbf-121">Header</span></span>|<span data-ttu-id="1dcbf-122">Valor</span><span class="sxs-lookup"><span data-stu-id="1dcbf-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="1dcbf-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="1dcbf-123">Authorization</span></span>|<span data-ttu-id="1dcbf-124">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="1dcbf-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="1dcbf-125">Accept</span><span class="sxs-lookup"><span data-stu-id="1dcbf-125">Accept</span></span>|<span data-ttu-id="1dcbf-126">application/json</span><span class="sxs-lookup"><span data-stu-id="1dcbf-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="1dcbf-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="1dcbf-127">Request body</span></span>
<span data-ttu-id="1dcbf-128">No corpo da solicitação, forneça uma representação JSON do objeto termsAndConditionsAcceptanceStatus.</span><span class="sxs-lookup"><span data-stu-id="1dcbf-128">In the request body, supply a JSON representation for the termsAndConditionsAcceptanceStatus object.</span></span>

<span data-ttu-id="1dcbf-129">A tabela a seguir mostra as propriedades que são necessárias ao criar termsAndConditionsAcceptanceStatus.</span><span class="sxs-lookup"><span data-stu-id="1dcbf-129">The following table shows the properties that are required when you create the termsAndConditionsAcceptanceStatus.</span></span>

|<span data-ttu-id="1dcbf-130">Propriedade</span><span class="sxs-lookup"><span data-stu-id="1dcbf-130">Property</span></span>|<span data-ttu-id="1dcbf-131">Tipo</span><span class="sxs-lookup"><span data-stu-id="1dcbf-131">Type</span></span>|<span data-ttu-id="1dcbf-132">Descrição</span><span class="sxs-lookup"><span data-stu-id="1dcbf-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="1dcbf-133">id</span><span class="sxs-lookup"><span data-stu-id="1dcbf-133">id</span></span>|<span data-ttu-id="1dcbf-134">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="1dcbf-134">String</span></span>|<span data-ttu-id="1dcbf-135">Identificador exclusivo da entidade.</span><span class="sxs-lookup"><span data-stu-id="1dcbf-135">Unique identifier of the entity.</span></span>|
|<span data-ttu-id="1dcbf-136">userDisplayName</span><span class="sxs-lookup"><span data-stu-id="1dcbf-136">userDisplayName</span></span>|<span data-ttu-id="1dcbf-137">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="1dcbf-137">String</span></span>|<span data-ttu-id="1dcbf-138">Nome de exibição do usuário cuja aceitação a entidade representa.</span><span class="sxs-lookup"><span data-stu-id="1dcbf-138">Display name of the user whose acceptance the entity represents.</span></span>|
|<span data-ttu-id="1dcbf-139">acceptedVersion</span><span class="sxs-lookup"><span data-stu-id="1dcbf-139">acceptedVersion</span></span>|<span data-ttu-id="1dcbf-140">Int32</span><span class="sxs-lookup"><span data-stu-id="1dcbf-140">Int32</span></span>|<span data-ttu-id="1dcbf-141">Número da versão mais recente dos T&C aceitos pelo usuário.</span><span class="sxs-lookup"><span data-stu-id="1dcbf-141">Most recent version number of the T&C accepted by the user.</span></span>|
|<span data-ttu-id="1dcbf-142">acceptedDateTime</span><span class="sxs-lookup"><span data-stu-id="1dcbf-142">acceptedDateTime</span></span>|<span data-ttu-id="1dcbf-143">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="1dcbf-143">DateTimeOffset</span></span>|<span data-ttu-id="1dcbf-144">A data e a hora em que os termos foram aceitos pela última vez pelo usuário.</span><span class="sxs-lookup"><span data-stu-id="1dcbf-144">DateTime when the terms were last accepted by the user.</span></span>|



## <a name="response"></a><span data-ttu-id="1dcbf-145">Resposta</span><span class="sxs-lookup"><span data-stu-id="1dcbf-145">Response</span></span>
<span data-ttu-id="1dcbf-146">Se tiver êxito, este método retornará um código de resposta `201 Created` e um objeto [termsAndConditionsAcceptanceStatus](../resources/intune-companyterms-termsandconditionsacceptancestatus.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="1dcbf-146">If successful, this method returns a `201 Created` response code and a [termsAndConditionsAcceptanceStatus](../resources/intune-companyterms-termsandconditionsacceptancestatus.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="1dcbf-147">Exemplo</span><span class="sxs-lookup"><span data-stu-id="1dcbf-147">Example</span></span>
### <a name="request"></a><span data-ttu-id="1dcbf-148">Solicitação</span><span class="sxs-lookup"><span data-stu-id="1dcbf-148">Request</span></span>
<span data-ttu-id="1dcbf-149">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="1dcbf-149">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/termsAndConditions/{termsAndConditionsId}/acceptanceStatuses
Content-type: application/json
Content-length: 211

{
  "@odata.type": "#microsoft.graph.termsAndConditionsAcceptanceStatus",
  "userDisplayName": "User Display Name value",
  "acceptedVersion": 15,
  "acceptedDateTime": "2016-12-31T23:57:43.6165506-08:00"
}
```

### <a name="response"></a><span data-ttu-id="1dcbf-150">Resposta</span><span class="sxs-lookup"><span data-stu-id="1dcbf-150">Response</span></span>
<span data-ttu-id="1dcbf-p103">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="1dcbf-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 260

{
  "@odata.type": "#microsoft.graph.termsAndConditionsAcceptanceStatus",
  "id": "a045ce1a-ce1a-a045-1ace-45a01ace45a0",
  "userDisplayName": "User Display Name value",
  "acceptedVersion": 15,
  "acceptedDateTime": "2016-12-31T23:57:43.6165506-08:00"
}
```





