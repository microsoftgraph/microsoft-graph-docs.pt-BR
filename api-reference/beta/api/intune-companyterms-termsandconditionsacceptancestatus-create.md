---
title: Criar termsAndConditionsAcceptanceStatus
description: Cria um novo objeto termsAndConditionsAcceptanceStatus.
author: dougeby
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 507fb1c9a558a017baa4fd05f28585bcac4c4e81
ms.sourcegitcommit: bbcf074f0be9d5e02f84c290122850cc5968fb1f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/14/2020
ms.locfileid: "43436521"
---
# <a name="create-termsandconditionsacceptancestatus"></a><span data-ttu-id="ff661-103">Criar termsAndConditionsAcceptanceStatus</span><span class="sxs-lookup"><span data-stu-id="ff661-103">Create termsAndConditionsAcceptanceStatus</span></span>

<span data-ttu-id="ff661-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="ff661-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="ff661-105">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="ff661-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="ff661-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="ff661-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="ff661-107">Cria um novo objeto [termsAndConditionsAcceptanceStatus](../resources/intune-companyterms-termsandconditionsacceptancestatus.md).</span><span class="sxs-lookup"><span data-stu-id="ff661-107">Create a new [termsAndConditionsAcceptanceStatus](../resources/intune-companyterms-termsandconditionsacceptancestatus.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="ff661-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="ff661-108">Prerequisites</span></span>
<span data-ttu-id="ff661-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="ff661-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="ff661-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="ff661-111">Permission type</span></span>|<span data-ttu-id="ff661-112">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="ff661-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="ff661-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="ff661-113">Delegated (work or school account)</span></span>|<span data-ttu-id="ff661-114">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="ff661-114">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="ff661-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="ff661-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="ff661-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="ff661-116">Not supported.</span></span>|
|<span data-ttu-id="ff661-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="ff661-117">Application</span></span>|<span data-ttu-id="ff661-118">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="ff661-118">DeviceManagementServiceConfig.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="ff661-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="ff661-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/termsAndConditions/{termsAndConditionsId}/acceptanceStatuses
```

## <a name="request-headers"></a><span data-ttu-id="ff661-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="ff661-120">Request headers</span></span>
|<span data-ttu-id="ff661-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="ff661-121">Header</span></span>|<span data-ttu-id="ff661-122">Valor</span><span class="sxs-lookup"><span data-stu-id="ff661-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="ff661-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="ff661-123">Authorization</span></span>|<span data-ttu-id="ff661-124">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="ff661-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="ff661-125">Aceitar</span><span class="sxs-lookup"><span data-stu-id="ff661-125">Accept</span></span>|<span data-ttu-id="ff661-126">application/json</span><span class="sxs-lookup"><span data-stu-id="ff661-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="ff661-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="ff661-127">Request body</span></span>
<span data-ttu-id="ff661-128">No corpo da solicitação, forneça uma representação JSON do objeto termsAndConditionsAcceptanceStatus.</span><span class="sxs-lookup"><span data-stu-id="ff661-128">In the request body, supply a JSON representation for the termsAndConditionsAcceptanceStatus object.</span></span>

<span data-ttu-id="ff661-129">A tabela a seguir mostra as propriedades que são necessárias ao criar termsAndConditionsAcceptanceStatus.</span><span class="sxs-lookup"><span data-stu-id="ff661-129">The following table shows the properties that are required when you create the termsAndConditionsAcceptanceStatus.</span></span>

|<span data-ttu-id="ff661-130">Propriedade</span><span class="sxs-lookup"><span data-stu-id="ff661-130">Property</span></span>|<span data-ttu-id="ff661-131">Tipo</span><span class="sxs-lookup"><span data-stu-id="ff661-131">Type</span></span>|<span data-ttu-id="ff661-132">Descrição</span><span class="sxs-lookup"><span data-stu-id="ff661-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="ff661-133">id</span><span class="sxs-lookup"><span data-stu-id="ff661-133">id</span></span>|<span data-ttu-id="ff661-134">String</span><span class="sxs-lookup"><span data-stu-id="ff661-134">String</span></span>|<span data-ttu-id="ff661-135">Identificador exclusivo da entidade.</span><span class="sxs-lookup"><span data-stu-id="ff661-135">Unique identifier of the entity.</span></span>|
|<span data-ttu-id="ff661-136">userDisplayName</span><span class="sxs-lookup"><span data-stu-id="ff661-136">userDisplayName</span></span>|<span data-ttu-id="ff661-137">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="ff661-137">String</span></span>|<span data-ttu-id="ff661-138">Nome de exibição do usuário cuja aceitação a entidade representa.</span><span class="sxs-lookup"><span data-stu-id="ff661-138">Display name of the user whose acceptance the entity represents.</span></span>|
|<span data-ttu-id="ff661-139">acceptedVersion</span><span class="sxs-lookup"><span data-stu-id="ff661-139">acceptedVersion</span></span>|<span data-ttu-id="ff661-140">Int32</span><span class="sxs-lookup"><span data-stu-id="ff661-140">Int32</span></span>|<span data-ttu-id="ff661-141">Número da versão mais recente dos T&C aceitos pelo usuário.</span><span class="sxs-lookup"><span data-stu-id="ff661-141">Most recent version number of the T&C accepted by the user.</span></span>|
|<span data-ttu-id="ff661-142">acceptedDateTime</span><span class="sxs-lookup"><span data-stu-id="ff661-142">acceptedDateTime</span></span>|<span data-ttu-id="ff661-143">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="ff661-143">DateTimeOffset</span></span>|<span data-ttu-id="ff661-144">A data e a hora em que os termos foram aceitos pela última vez pelo usuário.</span><span class="sxs-lookup"><span data-stu-id="ff661-144">DateTime when the terms were last accepted by the user.</span></span>|
|<span data-ttu-id="ff661-145">userPrincipalName</span><span class="sxs-lookup"><span data-stu-id="ff661-145">userPrincipalName</span></span>|<span data-ttu-id="ff661-146">String</span><span class="sxs-lookup"><span data-stu-id="ff661-146">String</span></span>|<span data-ttu-id="ff661-147">O userPrincipalName do usuário que aceitou o termo.</span><span class="sxs-lookup"><span data-stu-id="ff661-147">The userPrincipalName of the User that accepted the term.</span></span>|



## <a name="response"></a><span data-ttu-id="ff661-148">Resposta</span><span class="sxs-lookup"><span data-stu-id="ff661-148">Response</span></span>
<span data-ttu-id="ff661-149">Se tiver êxito, este método retornará um código de resposta `201 Created` e um objeto [termsAndConditionsAcceptanceStatus](../resources/intune-companyterms-termsandconditionsacceptancestatus.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="ff661-149">If successful, this method returns a `201 Created` response code and a [termsAndConditionsAcceptanceStatus](../resources/intune-companyterms-termsandconditionsacceptancestatus.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="ff661-150">Exemplo</span><span class="sxs-lookup"><span data-stu-id="ff661-150">Example</span></span>

### <a name="request"></a><span data-ttu-id="ff661-151">Solicitação</span><span class="sxs-lookup"><span data-stu-id="ff661-151">Request</span></span>
<span data-ttu-id="ff661-152">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="ff661-152">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/termsAndConditions/{termsAndConditionsId}/acceptanceStatuses
Content-type: application/json
Content-length: 264

{
  "@odata.type": "#microsoft.graph.termsAndConditionsAcceptanceStatus",
  "userDisplayName": "User Display Name value",
  "acceptedVersion": 15,
  "acceptedDateTime": "2016-12-31T23:57:43.6165506-08:00",
  "userPrincipalName": "User Principal Name value"
}
```

### <a name="response"></a><span data-ttu-id="ff661-153">Resposta</span><span class="sxs-lookup"><span data-stu-id="ff661-153">Response</span></span>
<span data-ttu-id="ff661-p102">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="ff661-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 313

{
  "@odata.type": "#microsoft.graph.termsAndConditionsAcceptanceStatus",
  "id": "a045ce1a-ce1a-a045-1ace-45a01ace45a0",
  "userDisplayName": "User Display Name value",
  "acceptedVersion": 15,
  "acceptedDateTime": "2016-12-31T23:57:43.6165506-08:00",
  "userPrincipalName": "User Principal Name value"
}
```



