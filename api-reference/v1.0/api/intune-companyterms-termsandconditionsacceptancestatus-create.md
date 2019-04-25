---
title: Criar termsAndConditionsAcceptanceStatus
description: Cria um novo objeto termsAndConditionsAcceptanceStatus.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 69ea9a95599c225a80d1902fa3d0de720f9a9f82
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/24/2019
ms.locfileid: "32542036"
---
# <a name="create-termsandconditionsacceptancestatus"></a><span data-ttu-id="1d2c3-103">Criar termsAndConditionsAcceptanceStatus</span><span class="sxs-lookup"><span data-stu-id="1d2c3-103">Create termsAndConditionsAcceptanceStatus</span></span>

> <span data-ttu-id="1d2c3-104">**Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="1d2c3-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="1d2c3-105">Cria um novo objeto [termsAndConditionsAcceptanceStatus](../resources/intune-companyterms-termsandconditionsacceptancestatus.md).</span><span class="sxs-lookup"><span data-stu-id="1d2c3-105">Create a new [termsAndConditionsAcceptanceStatus](../resources/intune-companyterms-termsandconditionsacceptancestatus.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="1d2c3-106">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="1d2c3-106">Prerequisites</span></span>
<span data-ttu-id="1d2c3-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="1d2c3-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="1d2c3-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="1d2c3-109">Permission type</span></span>|<span data-ttu-id="1d2c3-110">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="1d2c3-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="1d2c3-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="1d2c3-111">Delegated (work or school account)</span></span>|<span data-ttu-id="1d2c3-112">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="1d2c3-112">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="1d2c3-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="1d2c3-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="1d2c3-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="1d2c3-114">Not supported.</span></span>|
|<span data-ttu-id="1d2c3-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="1d2c3-115">Application</span></span>|<span data-ttu-id="1d2c3-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="1d2c3-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="1d2c3-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="1d2c3-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/termsAndConditions/{termsAndConditionsId}/acceptanceStatuses
```

## <a name="request-headers"></a><span data-ttu-id="1d2c3-118">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="1d2c3-118">Request headers</span></span>
|<span data-ttu-id="1d2c3-119">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="1d2c3-119">Header</span></span>|<span data-ttu-id="1d2c3-120">Valor</span><span class="sxs-lookup"><span data-stu-id="1d2c3-120">Value</span></span>|
|:---|:---|
|<span data-ttu-id="1d2c3-121">Autorização</span><span class="sxs-lookup"><span data-stu-id="1d2c3-121">Authorization</span></span>|<span data-ttu-id="1d2c3-122">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="1d2c3-122">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="1d2c3-123">Aceitar</span><span class="sxs-lookup"><span data-stu-id="1d2c3-123">Accept</span></span>|<span data-ttu-id="1d2c3-124">application/json</span><span class="sxs-lookup"><span data-stu-id="1d2c3-124">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="1d2c3-125">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="1d2c3-125">Request body</span></span>
<span data-ttu-id="1d2c3-126">No corpo da solicitação, forneça uma representação JSON do objeto termsAndConditionsAcceptanceStatus.</span><span class="sxs-lookup"><span data-stu-id="1d2c3-126">In the request body, supply a JSON representation for the termsAndConditionsAcceptanceStatus object.</span></span>

<span data-ttu-id="1d2c3-127">A tabela a seguir mostra as propriedades que são necessárias ao criar termsAndConditionsAcceptanceStatus.</span><span class="sxs-lookup"><span data-stu-id="1d2c3-127">The following table shows the properties that are required when you create the termsAndConditionsAcceptanceStatus.</span></span>

|<span data-ttu-id="1d2c3-128">Propriedade</span><span class="sxs-lookup"><span data-stu-id="1d2c3-128">Property</span></span>|<span data-ttu-id="1d2c3-129">Tipo</span><span class="sxs-lookup"><span data-stu-id="1d2c3-129">Type</span></span>|<span data-ttu-id="1d2c3-130">Descrição</span><span class="sxs-lookup"><span data-stu-id="1d2c3-130">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="1d2c3-131">id</span><span class="sxs-lookup"><span data-stu-id="1d2c3-131">id</span></span>|<span data-ttu-id="1d2c3-132">String</span><span class="sxs-lookup"><span data-stu-id="1d2c3-132">String</span></span>|<span data-ttu-id="1d2c3-133">Identificador exclusivo da entidade.</span><span class="sxs-lookup"><span data-stu-id="1d2c3-133">Unique identifier of the entity.</span></span>|
|<span data-ttu-id="1d2c3-134">userDisplayName</span><span class="sxs-lookup"><span data-stu-id="1d2c3-134">userDisplayName</span></span>|<span data-ttu-id="1d2c3-135">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="1d2c3-135">String</span></span>|<span data-ttu-id="1d2c3-136">Nome de exibição do usuário cuja aceitação a entidade representa.</span><span class="sxs-lookup"><span data-stu-id="1d2c3-136">Display name of the user whose acceptance the entity represents.</span></span>|
|<span data-ttu-id="1d2c3-137">acceptedVersion</span><span class="sxs-lookup"><span data-stu-id="1d2c3-137">acceptedVersion</span></span>|<span data-ttu-id="1d2c3-138">Int32</span><span class="sxs-lookup"><span data-stu-id="1d2c3-138">Int32</span></span>|<span data-ttu-id="1d2c3-139">Número da versão mais recente dos T&C aceitos pelo usuário.</span><span class="sxs-lookup"><span data-stu-id="1d2c3-139">Most recent version number of the T&C accepted by the user.</span></span>|
|<span data-ttu-id="1d2c3-140">acceptedDateTime</span><span class="sxs-lookup"><span data-stu-id="1d2c3-140">acceptedDateTime</span></span>|<span data-ttu-id="1d2c3-141">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="1d2c3-141">DateTimeOffset</span></span>|<span data-ttu-id="1d2c3-142">A data e a hora em que os termos foram aceitos pela última vez pelo usuário.</span><span class="sxs-lookup"><span data-stu-id="1d2c3-142">DateTime when the terms were last accepted by the user.</span></span>|



## <a name="response"></a><span data-ttu-id="1d2c3-143">Resposta</span><span class="sxs-lookup"><span data-stu-id="1d2c3-143">Response</span></span>
<span data-ttu-id="1d2c3-144">Se tiver êxito, este método retornará um código de resposta `201 Created` e um objeto [termsAndConditionsAcceptanceStatus](../resources/intune-companyterms-termsandconditionsacceptancestatus.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="1d2c3-144">If successful, this method returns a `201 Created` response code and a [termsAndConditionsAcceptanceStatus](../resources/intune-companyterms-termsandconditionsacceptancestatus.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="1d2c3-145">Exemplo</span><span class="sxs-lookup"><span data-stu-id="1d2c3-145">Example</span></span>

### <a name="request"></a><span data-ttu-id="1d2c3-146">Solicitação</span><span class="sxs-lookup"><span data-stu-id="1d2c3-146">Request</span></span>
<span data-ttu-id="1d2c3-147">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="1d2c3-147">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/v1.0/deviceManagement/termsAndConditions/{termsAndConditionsId}/acceptanceStatuses
Content-type: application/json
Content-length: 211

{
  "@odata.type": "#microsoft.graph.termsAndConditionsAcceptanceStatus",
  "userDisplayName": "User Display Name value",
  "acceptedVersion": 15,
  "acceptedDateTime": "2016-12-31T23:57:43.6165506-08:00"
}
```

### <a name="response"></a><span data-ttu-id="1d2c3-148">Resposta</span><span class="sxs-lookup"><span data-stu-id="1d2c3-148">Response</span></span>
<span data-ttu-id="1d2c3-p102">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="1d2c3-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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



