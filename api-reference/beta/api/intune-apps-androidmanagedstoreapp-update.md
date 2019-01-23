---
title: Atualizar androidManagedStoreApp
description: Atualize as propriedades de um objeto androidManagedStoreApp.
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: 9d100738e96219dff925f069259309b2ffccb84a
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/23/2019
ms.locfileid: "29413763"
---
# <a name="update-androidmanagedstoreapp"></a><span data-ttu-id="9876b-103">Atualizar androidManagedStoreApp</span><span class="sxs-lookup"><span data-stu-id="9876b-103">Update androidManagedStoreApp</span></span>

> <span data-ttu-id="9876b-104">**Importante:** APIs sob a versão /beta no Microsoft Graph estão sujeitos a alterações.</span><span class="sxs-lookup"><span data-stu-id="9876b-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="9876b-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="9876b-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="9876b-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença de Intune ativa](https://go.microsoft.com/fwlink/?linkid=839381) para o inquilino.</span><span class="sxs-lookup"><span data-stu-id="9876b-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="9876b-107">Atualize as propriedades de um objeto [androidManagedStoreApp](../resources/intune-apps-androidmanagedstoreapp.md) .</span><span class="sxs-lookup"><span data-stu-id="9876b-107">Update the properties of a [androidManagedStoreApp](../resources/intune-apps-androidmanagedstoreapp.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="9876b-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="9876b-108">Prerequisites</span></span>
<span data-ttu-id="9876b-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/concepts/permissions-reference.md).</span><span class="sxs-lookup"><span data-stu-id="9876b-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="9876b-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="9876b-111">Permission type</span></span>|<span data-ttu-id="9876b-112">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="9876b-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="9876b-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="9876b-113">Delegated (work or school account)</span></span>|<span data-ttu-id="9876b-114">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="9876b-114">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="9876b-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="9876b-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="9876b-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="9876b-116">Not supported.</span></span>|
|<span data-ttu-id="9876b-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="9876b-117">Application</span></span>|<span data-ttu-id="9876b-118">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="9876b-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="9876b-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="9876b-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceAppManagement/mobileApps/{mobileAppId}
PATCH /deviceAppManagement/mobileApps/{mobileAppId}/userStatuses/{userAppInstallStatusId}/app
PATCH /deviceAppManagement/mobileApps/{mobileAppId}/deviceStatuses/{mobileAppInstallStatusId}/app
```

## <a name="request-headers"></a><span data-ttu-id="9876b-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="9876b-120">Request headers</span></span>
|<span data-ttu-id="9876b-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="9876b-121">Header</span></span>|<span data-ttu-id="9876b-122">Valor</span><span class="sxs-lookup"><span data-stu-id="9876b-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="9876b-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="9876b-123">Authorization</span></span>|<span data-ttu-id="9876b-124">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="9876b-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="9876b-125">Aceitar</span><span class="sxs-lookup"><span data-stu-id="9876b-125">Accept</span></span>|<span data-ttu-id="9876b-126">application/json</span><span class="sxs-lookup"><span data-stu-id="9876b-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="9876b-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="9876b-127">Request body</span></span>
<span data-ttu-id="9876b-128">No corpo da solicitação, fornece uma representação JSON para o objeto [androidManagedStoreApp](../resources/intune-apps-androidmanagedstoreapp.md) .</span><span class="sxs-lookup"><span data-stu-id="9876b-128">In the request body, supply a JSON representation for the [androidManagedStoreApp](../resources/intune-apps-androidmanagedstoreapp.md) object.</span></span>

<span data-ttu-id="9876b-129">A tabela a seguir mostra as propriedades que são necessárias quando você cria o [androidManagedStoreApp](../resources/intune-apps-androidmanagedstoreapp.md).</span><span class="sxs-lookup"><span data-stu-id="9876b-129">The following table shows the properties that are required when you create the [androidManagedStoreApp](../resources/intune-apps-androidmanagedstoreapp.md).</span></span>

|<span data-ttu-id="9876b-130">Propriedade</span><span class="sxs-lookup"><span data-stu-id="9876b-130">Property</span></span>|<span data-ttu-id="9876b-131">Tipo</span><span class="sxs-lookup"><span data-stu-id="9876b-131">Type</span></span>|<span data-ttu-id="9876b-132">Descrição</span><span class="sxs-lookup"><span data-stu-id="9876b-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="9876b-133">id</span><span class="sxs-lookup"><span data-stu-id="9876b-133">id</span></span>|<span data-ttu-id="9876b-134">String</span><span class="sxs-lookup"><span data-stu-id="9876b-134">String</span></span>|<span data-ttu-id="9876b-135">Chave da entidade.</span><span class="sxs-lookup"><span data-stu-id="9876b-135">Key of the entity.</span></span> <span data-ttu-id="9876b-136">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="9876b-136">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="9876b-137">displayName</span><span class="sxs-lookup"><span data-stu-id="9876b-137">displayName</span></span>|<span data-ttu-id="9876b-138">String</span><span class="sxs-lookup"><span data-stu-id="9876b-138">String</span></span>|<span data-ttu-id="9876b-139">O título do aplicativo importado ou definido pelo administrador.</span><span class="sxs-lookup"><span data-stu-id="9876b-139">The admin provided or imported title of the app.</span></span> <span data-ttu-id="9876b-140">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="9876b-140">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="9876b-141">description</span><span class="sxs-lookup"><span data-stu-id="9876b-141">description</span></span>|<span data-ttu-id="9876b-142">String</span><span class="sxs-lookup"><span data-stu-id="9876b-142">String</span></span>|<span data-ttu-id="9876b-143">A descrição do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="9876b-143">The description of the app.</span></span> <span data-ttu-id="9876b-144">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="9876b-144">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="9876b-145">publisher</span><span class="sxs-lookup"><span data-stu-id="9876b-145">publisher</span></span>|<span data-ttu-id="9876b-146">String</span><span class="sxs-lookup"><span data-stu-id="9876b-146">String</span></span>|<span data-ttu-id="9876b-147">O publicador do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="9876b-147">The publisher of the app.</span></span> <span data-ttu-id="9876b-148">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="9876b-148">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="9876b-149">largeIcon</span><span class="sxs-lookup"><span data-stu-id="9876b-149">largeIcon</span></span>|[<span data-ttu-id="9876b-150">mimeContent</span><span class="sxs-lookup"><span data-stu-id="9876b-150">mimeContent</span></span>](../resources/intune-shared-mimecontent.md)|<span data-ttu-id="9876b-151">O ícone grande, a ser exibido nos detalhes do aplicativo e usado para o carregamento do ícone.</span><span class="sxs-lookup"><span data-stu-id="9876b-151">The large icon, to be displayed in the app details and used for upload of the icon.</span></span> <span data-ttu-id="9876b-152">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="9876b-152">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="9876b-153">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="9876b-153">createdDateTime</span></span>|<span data-ttu-id="9876b-154">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="9876b-154">DateTimeOffset</span></span>|<span data-ttu-id="9876b-155">A data e a hora da criação do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="9876b-155">The date and time the app was created.</span></span> <span data-ttu-id="9876b-156">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="9876b-156">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="9876b-157">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="9876b-157">lastModifiedDateTime</span></span>|<span data-ttu-id="9876b-158">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="9876b-158">DateTimeOffset</span></span>|<span data-ttu-id="9876b-159">A data e a hora que o aplicativo foi modificado pela última vez.</span><span class="sxs-lookup"><span data-stu-id="9876b-159">The date and time the app was last modified.</span></span> <span data-ttu-id="9876b-160">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="9876b-160">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="9876b-161">isFeatured</span><span class="sxs-lookup"><span data-stu-id="9876b-161">isFeatured</span></span>|<span data-ttu-id="9876b-162">Boolean</span><span class="sxs-lookup"><span data-stu-id="9876b-162">Boolean</span></span>|<span data-ttu-id="9876b-163">O valor que indica se o aplicativo está marcado como em destaque pelo administrador. Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="9876b-163">The value indicating whether the app is marked as featured by the admin. Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="9876b-164">privacyInformationUrl</span><span class="sxs-lookup"><span data-stu-id="9876b-164">privacyInformationUrl</span></span>|<span data-ttu-id="9876b-165">String</span><span class="sxs-lookup"><span data-stu-id="9876b-165">String</span></span>|<span data-ttu-id="9876b-166">A URL da declaração de privacidade.</span><span class="sxs-lookup"><span data-stu-id="9876b-166">The privacy statement Url.</span></span> <span data-ttu-id="9876b-167">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="9876b-167">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="9876b-168">informationUrl</span><span class="sxs-lookup"><span data-stu-id="9876b-168">informationUrl</span></span>|<span data-ttu-id="9876b-169">String</span><span class="sxs-lookup"><span data-stu-id="9876b-169">String</span></span>|<span data-ttu-id="9876b-170">A URL de informações adicionais.</span><span class="sxs-lookup"><span data-stu-id="9876b-170">The more information Url.</span></span> <span data-ttu-id="9876b-171">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="9876b-171">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="9876b-172">owner</span><span class="sxs-lookup"><span data-stu-id="9876b-172">owner</span></span>|<span data-ttu-id="9876b-173">String</span><span class="sxs-lookup"><span data-stu-id="9876b-173">String</span></span>|<span data-ttu-id="9876b-174">O proprietário do conteúdo.</span><span class="sxs-lookup"><span data-stu-id="9876b-174">The owner of the app.</span></span> <span data-ttu-id="9876b-175">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="9876b-175">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="9876b-176">developer</span><span class="sxs-lookup"><span data-stu-id="9876b-176">developer</span></span>|<span data-ttu-id="9876b-177">String</span><span class="sxs-lookup"><span data-stu-id="9876b-177">String</span></span>|<span data-ttu-id="9876b-178">O desenvolvedor do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="9876b-178">The developer of the app.</span></span> <span data-ttu-id="9876b-179">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="9876b-179">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="9876b-180">Observações</span><span class="sxs-lookup"><span data-stu-id="9876b-180">notes</span></span>|<span data-ttu-id="9876b-181">String</span><span class="sxs-lookup"><span data-stu-id="9876b-181">String</span></span>|<span data-ttu-id="9876b-182">Anotações para o aplicativo.</span><span class="sxs-lookup"><span data-stu-id="9876b-182">Notes for the app.</span></span> <span data-ttu-id="9876b-183">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="9876b-183">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="9876b-184">uploadState</span><span class="sxs-lookup"><span data-stu-id="9876b-184">uploadState</span></span>|<span data-ttu-id="9876b-185">Int32</span><span class="sxs-lookup"><span data-stu-id="9876b-185">Int32</span></span>|<span data-ttu-id="9876b-186">O estado de carregamento.</span><span class="sxs-lookup"><span data-stu-id="9876b-186">The upload state.</span></span> <span data-ttu-id="9876b-187">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="9876b-187">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="9876b-188">publishingState</span><span class="sxs-lookup"><span data-stu-id="9876b-188">publishingState</span></span>|[<span data-ttu-id="9876b-189">mobileAppPublishingState</span><span class="sxs-lookup"><span data-stu-id="9876b-189">mobileAppPublishingState</span></span>](../resources/intune-apps-mobileapppublishingstate.md)|<span data-ttu-id="9876b-190">O estado de publicação para o aplicativo.</span><span class="sxs-lookup"><span data-stu-id="9876b-190">The publishing state for the app.</span></span> <span data-ttu-id="9876b-191">O aplicativo não pode ser assinado, a menos que ele seja publicado.</span><span class="sxs-lookup"><span data-stu-id="9876b-191">The app cannot be assigned unless the app is published.</span></span> <span data-ttu-id="9876b-192">Herdada do [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="9876b-192">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md).</span></span> <span data-ttu-id="9876b-193">Os valores possíveis são: `notPublished`, `processing`, `published`.</span><span class="sxs-lookup"><span data-stu-id="9876b-193">Possible values are: `notPublished`, `processing`, `published`.</span></span>|
|<span data-ttu-id="9876b-194">isAssigned</span><span class="sxs-lookup"><span data-stu-id="9876b-194">isAssigned</span></span>|<span data-ttu-id="9876b-195">Boolean</span><span class="sxs-lookup"><span data-stu-id="9876b-195">Boolean</span></span>|<span data-ttu-id="9876b-196">O valor que indica se o aplicativo é atribuído a pelo menos um grupo.</span><span class="sxs-lookup"><span data-stu-id="9876b-196">The value indicating whether the app is assigned to at least one group.</span></span> <span data-ttu-id="9876b-197">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="9876b-197">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="9876b-198">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="9876b-198">roleScopeTagIds</span></span>|<span data-ttu-id="9876b-199">String collection</span><span class="sxs-lookup"><span data-stu-id="9876b-199">String collection</span></span>|<span data-ttu-id="9876b-200">Lista de ids de marca de escopo para esse aplicativo móvel.</span><span class="sxs-lookup"><span data-stu-id="9876b-200">List of scope tag ids for this mobile app.</span></span> <span data-ttu-id="9876b-201">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="9876b-201">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="9876b-202">packageId</span><span class="sxs-lookup"><span data-stu-id="9876b-202">packageId</span></span>|<span data-ttu-id="9876b-203">String</span><span class="sxs-lookup"><span data-stu-id="9876b-203">String</span></span>|<span data-ttu-id="9876b-204">O identificador do pacote.</span><span class="sxs-lookup"><span data-stu-id="9876b-204">The package identifier.</span></span>|
|<span data-ttu-id="9876b-205">appIdentifier</span><span class="sxs-lookup"><span data-stu-id="9876b-205">appIdentifier</span></span>|<span data-ttu-id="9876b-206">String</span><span class="sxs-lookup"><span data-stu-id="9876b-206">String</span></span>|<span data-ttu-id="9876b-207">O Nome da Identidade.</span><span class="sxs-lookup"><span data-stu-id="9876b-207">The Identity Name.</span></span>|
|<span data-ttu-id="9876b-208">usedLicenseCount</span><span class="sxs-lookup"><span data-stu-id="9876b-208">usedLicenseCount</span></span>|<span data-ttu-id="9876b-209">Int32</span><span class="sxs-lookup"><span data-stu-id="9876b-209">Int32</span></span>|<span data-ttu-id="9876b-210">O número de aplicativos VPP em uso.</span><span class="sxs-lookup"><span data-stu-id="9876b-210">The number of VPP licenses in use.</span></span>|
|<span data-ttu-id="9876b-211">totalLicenseCount</span><span class="sxs-lookup"><span data-stu-id="9876b-211">totalLicenseCount</span></span>|<span data-ttu-id="9876b-212">Int32</span><span class="sxs-lookup"><span data-stu-id="9876b-212">Int32</span></span>|<span data-ttu-id="9876b-213">O número total de licenças VPP.</span><span class="sxs-lookup"><span data-stu-id="9876b-213">The total number of VPP licenses.</span></span>|
|<span data-ttu-id="9876b-214">appStoreUrl</span><span class="sxs-lookup"><span data-stu-id="9876b-214">appStoreUrl</span></span>|<span data-ttu-id="9876b-215">String</span><span class="sxs-lookup"><span data-stu-id="9876b-215">String</span></span>|<span data-ttu-id="9876b-216">Tocar para a URL do aplicativo de repositório de trabalho.</span><span class="sxs-lookup"><span data-stu-id="9876b-216">The Play for Work Store app URL.</span></span>|



## <a name="response"></a><span data-ttu-id="9876b-217">Resposta</span><span class="sxs-lookup"><span data-stu-id="9876b-217">Response</span></span>
<span data-ttu-id="9876b-218">Se tiver êxito, este método retornará um `200 OK` código de resposta e um objeto atualizado [androidManagedStoreApp](../resources/intune-apps-androidmanagedstoreapp.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="9876b-218">If successful, this method returns a `200 OK` response code and an updated [androidManagedStoreApp](../resources/intune-apps-androidmanagedstoreapp.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="9876b-219">Exemplo</span><span class="sxs-lookup"><span data-stu-id="9876b-219">Example</span></span>

### <a name="request"></a><span data-ttu-id="9876b-220">Solicitação</span><span class="sxs-lookup"><span data-stu-id="9876b-220">Request</span></span>
<span data-ttu-id="9876b-221">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="9876b-221">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceAppManagement/mobileApps/{mobileAppId}
Content-type: application/json
Content-length: 881

{
  "@odata.type": "#microsoft.graph.androidManagedStoreApp",
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
  "uploadState": 11,
  "publishingState": "processing",
  "isAssigned": true,
  "roleScopeTagIds": [
    "Role Scope Tag Ids value"
  ],
  "packageId": "Package Id value",
  "appIdentifier": "App Identifier value",
  "usedLicenseCount": 0,
  "totalLicenseCount": 1,
  "appStoreUrl": "https://example.com/appStoreUrl/"
}
```

### <a name="response"></a><span data-ttu-id="9876b-222">Resposta</span><span class="sxs-lookup"><span data-stu-id="9876b-222">Response</span></span>
<span data-ttu-id="9876b-p119">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="9876b-p119">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 1053

{
  "@odata.type": "#microsoft.graph.androidManagedStoreApp",
  "id": "87247525-7525-8724-2575-248725752487",
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
  "uploadState": 11,
  "publishingState": "processing",
  "isAssigned": true,
  "roleScopeTagIds": [
    "Role Scope Tag Ids value"
  ],
  "packageId": "Package Id value",
  "appIdentifier": "App Identifier value",
  "usedLicenseCount": 0,
  "totalLicenseCount": 1,
  "appStoreUrl": "https://example.com/appStoreUrl/"
}
```




