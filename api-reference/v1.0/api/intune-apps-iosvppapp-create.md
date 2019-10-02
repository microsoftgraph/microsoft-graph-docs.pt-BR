---
title: Criar iosVppApp
description: Cria um novo objeto iosVppApp.
author: davidmu1
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 1b2e582c99094399fa14c1316a8a3145b374a69c
ms.sourcegitcommit: bd5bb20856d4bffe93b2f77f131664849b602dbb
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 10/02/2019
ms.locfileid: "37358837"
---
# <a name="create-iosvppapp"></a><span data-ttu-id="61eaa-103">Criar iosVppApp</span><span class="sxs-lookup"><span data-stu-id="61eaa-103">Create iosVppApp</span></span>

> <span data-ttu-id="61eaa-104">**Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="61eaa-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="61eaa-105">Cria um novo objeto [iosVppApp](../resources/intune-apps-iosvppapp.md).</span><span class="sxs-lookup"><span data-stu-id="61eaa-105">Create a new [iosVppApp](../resources/intune-apps-iosvppapp.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="61eaa-106">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="61eaa-106">Prerequisites</span></span>
<span data-ttu-id="61eaa-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="61eaa-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="61eaa-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="61eaa-109">Permission type</span></span>|<span data-ttu-id="61eaa-110">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="61eaa-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="61eaa-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="61eaa-111">Delegated (work or school account)</span></span>|<span data-ttu-id="61eaa-112">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="61eaa-112">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="61eaa-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="61eaa-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="61eaa-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="61eaa-114">Not supported.</span></span>|
|<span data-ttu-id="61eaa-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="61eaa-115">Application</span></span>|<span data-ttu-id="61eaa-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="61eaa-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="61eaa-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="61eaa-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceAppManagement/mobileApps
```

## <a name="request-headers"></a><span data-ttu-id="61eaa-118">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="61eaa-118">Request headers</span></span>
|<span data-ttu-id="61eaa-119">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="61eaa-119">Header</span></span>|<span data-ttu-id="61eaa-120">Valor</span><span class="sxs-lookup"><span data-stu-id="61eaa-120">Value</span></span>|
|:---|:---|
|<span data-ttu-id="61eaa-121">Autorização</span><span class="sxs-lookup"><span data-stu-id="61eaa-121">Authorization</span></span>|<span data-ttu-id="61eaa-122">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="61eaa-122">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="61eaa-123">Aceitar</span><span class="sxs-lookup"><span data-stu-id="61eaa-123">Accept</span></span>|<span data-ttu-id="61eaa-124">application/json</span><span class="sxs-lookup"><span data-stu-id="61eaa-124">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="61eaa-125">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="61eaa-125">Request body</span></span>
<span data-ttu-id="61eaa-126">No corpo da solicitação, forneça uma representação JSON do objeto iosVppApp.</span><span class="sxs-lookup"><span data-stu-id="61eaa-126">In the request body, supply a JSON representation for the iosVppApp object.</span></span>

<span data-ttu-id="61eaa-127">A tabela a seguir mostra as propriedades obrigatórias ao criar iosVppApp.</span><span class="sxs-lookup"><span data-stu-id="61eaa-127">The following table shows the properties that are required when you create the iosVppApp.</span></span>

|<span data-ttu-id="61eaa-128">Propriedade</span><span class="sxs-lookup"><span data-stu-id="61eaa-128">Property</span></span>|<span data-ttu-id="61eaa-129">Tipo</span><span class="sxs-lookup"><span data-stu-id="61eaa-129">Type</span></span>|<span data-ttu-id="61eaa-130">Descrição</span><span class="sxs-lookup"><span data-stu-id="61eaa-130">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="61eaa-131">id</span><span class="sxs-lookup"><span data-stu-id="61eaa-131">id</span></span>|<span data-ttu-id="61eaa-132">String</span><span class="sxs-lookup"><span data-stu-id="61eaa-132">String</span></span>|<span data-ttu-id="61eaa-133">Chave da entidade.</span><span class="sxs-lookup"><span data-stu-id="61eaa-133">Key of the entity.</span></span> <span data-ttu-id="61eaa-134">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="61eaa-134">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="61eaa-135">displayName</span><span class="sxs-lookup"><span data-stu-id="61eaa-135">displayName</span></span>|<span data-ttu-id="61eaa-136">String</span><span class="sxs-lookup"><span data-stu-id="61eaa-136">String</span></span>|<span data-ttu-id="61eaa-137">O título do aplicativo importado ou definido pelo administrador.</span><span class="sxs-lookup"><span data-stu-id="61eaa-137">The admin provided or imported title of the app.</span></span> <span data-ttu-id="61eaa-138">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="61eaa-138">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="61eaa-139">descrição</span><span class="sxs-lookup"><span data-stu-id="61eaa-139">description</span></span>|<span data-ttu-id="61eaa-140">String</span><span class="sxs-lookup"><span data-stu-id="61eaa-140">String</span></span>|<span data-ttu-id="61eaa-141">A descrição do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="61eaa-141">The description of the app.</span></span> <span data-ttu-id="61eaa-142">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="61eaa-142">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="61eaa-143">publicador</span><span class="sxs-lookup"><span data-stu-id="61eaa-143">publisher</span></span>|<span data-ttu-id="61eaa-144">String</span><span class="sxs-lookup"><span data-stu-id="61eaa-144">String</span></span>|<span data-ttu-id="61eaa-145">O publicador do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="61eaa-145">The publisher of the app.</span></span> <span data-ttu-id="61eaa-146">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="61eaa-146">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="61eaa-147">largeIcon</span><span class="sxs-lookup"><span data-stu-id="61eaa-147">largeIcon</span></span>|[<span data-ttu-id="61eaa-148">mimeContent</span><span class="sxs-lookup"><span data-stu-id="61eaa-148">mimeContent</span></span>](../resources/intune-shared-mimecontent.md)|<span data-ttu-id="61eaa-149">O ícone grande, a ser exibido nos detalhes do aplicativo e usado para o carregamento do ícone.</span><span class="sxs-lookup"><span data-stu-id="61eaa-149">The large icon, to be displayed in the app details and used for upload of the icon.</span></span> <span data-ttu-id="61eaa-150">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="61eaa-150">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="61eaa-151">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="61eaa-151">createdDateTime</span></span>|<span data-ttu-id="61eaa-152">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="61eaa-152">DateTimeOffset</span></span>|<span data-ttu-id="61eaa-153">A data e a hora da criação do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="61eaa-153">The date and time the app was created.</span></span> <span data-ttu-id="61eaa-154">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="61eaa-154">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="61eaa-155">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="61eaa-155">lastModifiedDateTime</span></span>|<span data-ttu-id="61eaa-156">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="61eaa-156">DateTimeOffset</span></span>|<span data-ttu-id="61eaa-157">A data e a hora que o aplicativo foi modificado pela última vez.</span><span class="sxs-lookup"><span data-stu-id="61eaa-157">The date and time the app was last modified.</span></span> <span data-ttu-id="61eaa-158">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="61eaa-158">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="61eaa-159">isFeatured</span><span class="sxs-lookup"><span data-stu-id="61eaa-159">isFeatured</span></span>|<span data-ttu-id="61eaa-160">Boolean</span><span class="sxs-lookup"><span data-stu-id="61eaa-160">Boolean</span></span>|<span data-ttu-id="61eaa-161">O valor que indica se o aplicativo está marcado como em destaque pelo administrador. Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="61eaa-161">The value indicating whether the app is marked as featured by the admin. Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="61eaa-162">privacyInformationUrl</span><span class="sxs-lookup"><span data-stu-id="61eaa-162">privacyInformationUrl</span></span>|<span data-ttu-id="61eaa-163">String</span><span class="sxs-lookup"><span data-stu-id="61eaa-163">String</span></span>|<span data-ttu-id="61eaa-164">A URL da declaração de privacidade.</span><span class="sxs-lookup"><span data-stu-id="61eaa-164">The privacy statement Url.</span></span> <span data-ttu-id="61eaa-165">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="61eaa-165">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="61eaa-166">informationUrl</span><span class="sxs-lookup"><span data-stu-id="61eaa-166">informationUrl</span></span>|<span data-ttu-id="61eaa-167">String</span><span class="sxs-lookup"><span data-stu-id="61eaa-167">String</span></span>|<span data-ttu-id="61eaa-168">A URL de informações adicionais.</span><span class="sxs-lookup"><span data-stu-id="61eaa-168">The more information Url.</span></span> <span data-ttu-id="61eaa-169">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="61eaa-169">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="61eaa-170">owner</span><span class="sxs-lookup"><span data-stu-id="61eaa-170">owner</span></span>|<span data-ttu-id="61eaa-171">String</span><span class="sxs-lookup"><span data-stu-id="61eaa-171">String</span></span>|<span data-ttu-id="61eaa-172">O proprietário do conteúdo.</span><span class="sxs-lookup"><span data-stu-id="61eaa-172">The owner of the app.</span></span> <span data-ttu-id="61eaa-173">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="61eaa-173">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="61eaa-174">developer</span><span class="sxs-lookup"><span data-stu-id="61eaa-174">developer</span></span>|<span data-ttu-id="61eaa-175">String</span><span class="sxs-lookup"><span data-stu-id="61eaa-175">String</span></span>|<span data-ttu-id="61eaa-176">O desenvolvedor do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="61eaa-176">The developer of the app.</span></span> <span data-ttu-id="61eaa-177">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="61eaa-177">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="61eaa-178">notes</span><span class="sxs-lookup"><span data-stu-id="61eaa-178">notes</span></span>|<span data-ttu-id="61eaa-179">String</span><span class="sxs-lookup"><span data-stu-id="61eaa-179">String</span></span>|<span data-ttu-id="61eaa-180">Anotações do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="61eaa-180">Notes for the app.</span></span> <span data-ttu-id="61eaa-181">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="61eaa-181">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="61eaa-182">publishingState</span><span class="sxs-lookup"><span data-stu-id="61eaa-182">publishingState</span></span>|[<span data-ttu-id="61eaa-183">mobileAppPublishingState</span><span class="sxs-lookup"><span data-stu-id="61eaa-183">mobileAppPublishingState</span></span>](../resources/intune-apps-mobileapppublishingstate.md)|<span data-ttu-id="61eaa-184">O estado de publicação do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="61eaa-184">The publishing state for the app.</span></span> <span data-ttu-id="61eaa-185">O aplicativo não pode ser assinado, a menos que ele seja publicado.</span><span class="sxs-lookup"><span data-stu-id="61eaa-185">The app cannot be assigned unless the app is published.</span></span> <span data-ttu-id="61eaa-186">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="61eaa-186">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md).</span></span> <span data-ttu-id="61eaa-187">Os valores possíveis são: `notPublished`, `processing`, `published`.</span><span class="sxs-lookup"><span data-stu-id="61eaa-187">Possible values are: `notPublished`, `processing`, `published`.</span></span>|
|<span data-ttu-id="61eaa-188">usedLicenseCount</span><span class="sxs-lookup"><span data-stu-id="61eaa-188">usedLicenseCount</span></span>|<span data-ttu-id="61eaa-189">Int32</span><span class="sxs-lookup"><span data-stu-id="61eaa-189">Int32</span></span>|<span data-ttu-id="61eaa-190">O número de aplicativos VPP em uso.</span><span class="sxs-lookup"><span data-stu-id="61eaa-190">The number of VPP licenses in use.</span></span>|
|<span data-ttu-id="61eaa-191">totalLicenseCount</span><span class="sxs-lookup"><span data-stu-id="61eaa-191">totalLicenseCount</span></span>|<span data-ttu-id="61eaa-192">Int32</span><span class="sxs-lookup"><span data-stu-id="61eaa-192">Int32</span></span>|<span data-ttu-id="61eaa-193">O número total de licenças VPP.</span><span class="sxs-lookup"><span data-stu-id="61eaa-193">The total number of VPP licenses.</span></span>|
|<span data-ttu-id="61eaa-194">releaseDateTime</span><span class="sxs-lookup"><span data-stu-id="61eaa-194">releaseDateTime</span></span>|<span data-ttu-id="61eaa-195">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="61eaa-195">DateTimeOffset</span></span>|<span data-ttu-id="61eaa-196">A data e a hora de lançamento do aplicativo VPP.</span><span class="sxs-lookup"><span data-stu-id="61eaa-196">The VPP application release date and time.</span></span>|
|<span data-ttu-id="61eaa-197">appStoreUrl</span><span class="sxs-lookup"><span data-stu-id="61eaa-197">appStoreUrl</span></span>|<span data-ttu-id="61eaa-198">String</span><span class="sxs-lookup"><span data-stu-id="61eaa-198">String</span></span>|<span data-ttu-id="61eaa-199">A URL da loja.</span><span class="sxs-lookup"><span data-stu-id="61eaa-199">The store URL.</span></span>|
|<span data-ttu-id="61eaa-200">licensingType</span><span class="sxs-lookup"><span data-stu-id="61eaa-200">licensingType</span></span>|[<span data-ttu-id="61eaa-201">vppLicensingType</span><span class="sxs-lookup"><span data-stu-id="61eaa-201">vppLicensingType</span></span>](../resources/intune-apps-vpplicensingtype.md)|<span data-ttu-id="61eaa-202">O tipo de licença com suporte.</span><span class="sxs-lookup"><span data-stu-id="61eaa-202">The supported License Type.</span></span>|
|<span data-ttu-id="61eaa-203">applicableDeviceType</span><span class="sxs-lookup"><span data-stu-id="61eaa-203">applicableDeviceType</span></span>|[<span data-ttu-id="61eaa-204">iosDeviceType</span><span class="sxs-lookup"><span data-stu-id="61eaa-204">iosDeviceType</span></span>](../resources/intune-apps-iosdevicetype.md)|<span data-ttu-id="61eaa-205">O tipo de dispositivo iOS aplicável.</span><span class="sxs-lookup"><span data-stu-id="61eaa-205">The applicable iOS Device Type.</span></span>|
|<span data-ttu-id="61eaa-206">vppTokenOrganizationName</span><span class="sxs-lookup"><span data-stu-id="61eaa-206">vppTokenOrganizationName</span></span>|<span data-ttu-id="61eaa-207">String</span><span class="sxs-lookup"><span data-stu-id="61eaa-207">String</span></span>|<span data-ttu-id="61eaa-208">A organização associada ao Token do Programa de Compra por Volume da Apple</span><span class="sxs-lookup"><span data-stu-id="61eaa-208">The organization associated with the Apple Volume Purchase Program Token</span></span>|
|<span data-ttu-id="61eaa-209">vppTokenAccountType</span><span class="sxs-lookup"><span data-stu-id="61eaa-209">vppTokenAccountType</span></span>|[<span data-ttu-id="61eaa-210">vppTokenAccountType</span><span class="sxs-lookup"><span data-stu-id="61eaa-210">vppTokenAccountType</span></span>](../resources/intune-shared-vpptokenaccounttype.md)|<span data-ttu-id="61eaa-211">O tipo de programa de compra por volume ao qual o Token do Programa de Compra por Volume da Apple especificado está associado.</span><span class="sxs-lookup"><span data-stu-id="61eaa-211">The type of volume purchase program which the given Apple Volume Purchase Program Token is associated with.</span></span> <span data-ttu-id="61eaa-212">Os valores possíveis são: `business` e `education`.</span><span class="sxs-lookup"><span data-stu-id="61eaa-212">Possible values are: `business`, `education`.</span></span> <span data-ttu-id="61eaa-213">Os valores possíveis são: `business`, `education`.</span><span class="sxs-lookup"><span data-stu-id="61eaa-213">Possible values are: `business`, `education`.</span></span>|
|<span data-ttu-id="61eaa-214">vppTokenAppleId</span><span class="sxs-lookup"><span data-stu-id="61eaa-214">vppTokenAppleId</span></span>|<span data-ttu-id="61eaa-215">String</span><span class="sxs-lookup"><span data-stu-id="61eaa-215">String</span></span>|<span data-ttu-id="61eaa-216">O Apple Id associado ao Token do Programa de Compra de Volume da Apple.</span><span class="sxs-lookup"><span data-stu-id="61eaa-216">The Apple Id associated with the given Apple Volume Purchase Program Token.</span></span>|
|<span data-ttu-id="61eaa-217">bundleId</span><span class="sxs-lookup"><span data-stu-id="61eaa-217">bundleId</span></span>|<span data-ttu-id="61eaa-218">String</span><span class="sxs-lookup"><span data-stu-id="61eaa-218">String</span></span>|<span data-ttu-id="61eaa-219">O Nome da Identidade.</span><span class="sxs-lookup"><span data-stu-id="61eaa-219">The Identity Name.</span></span>|



## <a name="response"></a><span data-ttu-id="61eaa-220">Resposta</span><span class="sxs-lookup"><span data-stu-id="61eaa-220">Response</span></span>
<span data-ttu-id="61eaa-221">Se tiver êxito, este método retornará o código de resposta `201 Created` e o objeto [iosVppApp](../resources/intune-apps-iosvppapp.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="61eaa-221">If successful, this method returns a `201 Created` response code and a [iosVppApp](../resources/intune-apps-iosvppapp.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="61eaa-222">Exemplo</span><span class="sxs-lookup"><span data-stu-id="61eaa-222">Example</span></span>

### <a name="request"></a><span data-ttu-id="61eaa-223">Solicitação</span><span class="sxs-lookup"><span data-stu-id="61eaa-223">Request</span></span>
<span data-ttu-id="61eaa-224">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="61eaa-224">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/v1.0/deviceAppManagement/mobileApps
Content-type: application/json
Content-length: 1222

{
  "@odata.type": "#microsoft.graph.iosVppApp",
  "displayName": "Display Name value",
  "description": "Description value",
  "publisher": "Publisher value",
  "largeIcon": {
    "@odata.type": "microsoft.graph.mimeContent",
    "type": "Type value",
    "value": "dmFsdWU="
  },
  "isFeatured": true,
  "privacyInformationUrl": "https://example.com/privacyInformationUrl/",
  "informationUrl": "https://example.com/informationUrl/",
  "owner": "Owner value",
  "developer": "Developer value",
  "notes": "Notes value",
  "publishingState": "processing",
  "usedLicenseCount": 0,
  "totalLicenseCount": 1,
  "releaseDateTime": "2017-01-01T00:01:34.7470482-08:00",
  "appStoreUrl": "https://example.com/appStoreUrl/",
  "licensingType": {
    "@odata.type": "microsoft.graph.vppLicensingType",
    "supportsUserLicensing": true,
    "supportsDeviceLicensing": true
  },
  "applicableDeviceType": {
    "@odata.type": "microsoft.graph.iosDeviceType",
    "iPad": true,
    "iPhoneAndIPod": true
  },
  "vppTokenOrganizationName": "Vpp Token Organization Name value",
  "vppTokenAccountType": "education",
  "vppTokenAppleId": "Vpp Token Apple Id value",
  "bundleId": "Bundle Id value"
}
```

### <a name="response"></a><span data-ttu-id="61eaa-225">Resposta</span><span class="sxs-lookup"><span data-stu-id="61eaa-225">Response</span></span>
<span data-ttu-id="61eaa-p116">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="61eaa-p116">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 1394

{
  "@odata.type": "#microsoft.graph.iosVppApp",
  "id": "a0ac9b6f-9b6f-a0ac-6f9b-aca06f9baca0",
  "displayName": "Display Name value",
  "description": "Description value",
  "publisher": "Publisher value",
  "largeIcon": {
    "@odata.type": "microsoft.graph.mimeContent",
    "type": "Type value",
    "value": "dmFsdWU="
  },
  "createdDateTime": "2017-01-01T00:02:43.5775965-08:00",
  "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
  "isFeatured": true,
  "privacyInformationUrl": "https://example.com/privacyInformationUrl/",
  "informationUrl": "https://example.com/informationUrl/",
  "owner": "Owner value",
  "developer": "Developer value",
  "notes": "Notes value",
  "publishingState": "processing",
  "usedLicenseCount": 0,
  "totalLicenseCount": 1,
  "releaseDateTime": "2017-01-01T00:01:34.7470482-08:00",
  "appStoreUrl": "https://example.com/appStoreUrl/",
  "licensingType": {
    "@odata.type": "microsoft.graph.vppLicensingType",
    "supportsUserLicensing": true,
    "supportsDeviceLicensing": true
  },
  "applicableDeviceType": {
    "@odata.type": "microsoft.graph.iosDeviceType",
    "iPad": true,
    "iPhoneAndIPod": true
  },
  "vppTokenOrganizationName": "Vpp Token Organization Name value",
  "vppTokenAccountType": "education",
  "vppTokenAppleId": "Vpp Token Apple Id value",
  "bundleId": "Bundle Id value"
}
```




