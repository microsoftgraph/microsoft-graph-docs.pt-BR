---
title: Atualizar androidForWorkApp
description: Atualize as propriedades de um objeto androidForWorkApp.
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: 2bab6f4e9f042bff37284258eb025baf5077bf97
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/12/2019
ms.locfileid: "27960137"
---
# <a name="update-androidforworkapp"></a><span data-ttu-id="44dc1-103">Atualizar androidForWorkApp</span><span class="sxs-lookup"><span data-stu-id="44dc1-103">Update androidForWorkApp</span></span>

> <span data-ttu-id="44dc1-104">**Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="44dc1-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="44dc1-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="44dc1-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="44dc1-106">**Observação:** O uso das APIs do Microsoft Graph para configurar controles e políticas do Intune ainda exige que o serviço do Intune seja [corretamente licenciado](https://go.microsoft.com/fwlink/?linkid=839381) pelo cliente.</span><span class="sxs-lookup"><span data-stu-id="44dc1-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="44dc1-107">Atualize as propriedades de um objeto [androidForWorkApp](../resources/intune-apps-androidforworkapp.md) .</span><span class="sxs-lookup"><span data-stu-id="44dc1-107">Update the properties of a [androidForWorkApp](../resources/intune-apps-androidforworkapp.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="44dc1-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="44dc1-108">Prerequisites</span></span>
<span data-ttu-id="44dc1-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="44dc1-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="44dc1-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="44dc1-111">Permission type</span></span>|<span data-ttu-id="44dc1-112">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="44dc1-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="44dc1-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="44dc1-113">Delegated (work or school account)</span></span>|<span data-ttu-id="44dc1-114">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="44dc1-114">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="44dc1-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="44dc1-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="44dc1-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="44dc1-116">Not supported.</span></span>|
|<span data-ttu-id="44dc1-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="44dc1-117">Application</span></span>|<span data-ttu-id="44dc1-118">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="44dc1-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="44dc1-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="44dc1-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceAppManagement/mobileApps/{mobileAppId}
PATCH /deviceAppManagement/mobileApps/{mobileAppId}/userStatuses/{userAppInstallStatusId}/app
PATCH /deviceAppManagement/mobileApps/{mobileAppId}/deviceStatuses/{mobileAppInstallStatusId}/app
```

## <a name="request-headers"></a><span data-ttu-id="44dc1-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="44dc1-120">Request headers</span></span>
|<span data-ttu-id="44dc1-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="44dc1-121">Header</span></span>|<span data-ttu-id="44dc1-122">Valor</span><span class="sxs-lookup"><span data-stu-id="44dc1-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="44dc1-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="44dc1-123">Authorization</span></span>|<span data-ttu-id="44dc1-124">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="44dc1-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="44dc1-125">Aceitar</span><span class="sxs-lookup"><span data-stu-id="44dc1-125">Accept</span></span>|<span data-ttu-id="44dc1-126">application/json</span><span class="sxs-lookup"><span data-stu-id="44dc1-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="44dc1-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="44dc1-127">Request body</span></span>
<span data-ttu-id="44dc1-128">No corpo da solicitação, fornece uma representação JSON para o objeto [androidForWorkApp](../resources/intune-apps-androidforworkapp.md) .</span><span class="sxs-lookup"><span data-stu-id="44dc1-128">In the request body, supply a JSON representation for the [androidForWorkApp](../resources/intune-apps-androidforworkapp.md) object.</span></span>

<span data-ttu-id="44dc1-129">A tabela a seguir mostra as propriedades que são necessárias quando você cria o [androidForWorkApp](../resources/intune-apps-androidforworkapp.md).</span><span class="sxs-lookup"><span data-stu-id="44dc1-129">The following table shows the properties that are required when you create the [androidForWorkApp](../resources/intune-apps-androidforworkapp.md).</span></span>

|<span data-ttu-id="44dc1-130">Propriedade</span><span class="sxs-lookup"><span data-stu-id="44dc1-130">Property</span></span>|<span data-ttu-id="44dc1-131">Tipo</span><span class="sxs-lookup"><span data-stu-id="44dc1-131">Type</span></span>|<span data-ttu-id="44dc1-132">Descrição</span><span class="sxs-lookup"><span data-stu-id="44dc1-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="44dc1-133">id</span><span class="sxs-lookup"><span data-stu-id="44dc1-133">id</span></span>|<span data-ttu-id="44dc1-134">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="44dc1-134">String</span></span>|<span data-ttu-id="44dc1-135">Chave da entidade.</span><span class="sxs-lookup"><span data-stu-id="44dc1-135">Key of the entity.</span></span> <span data-ttu-id="44dc1-136">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="44dc1-136">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="44dc1-137">displayName</span><span class="sxs-lookup"><span data-stu-id="44dc1-137">displayName</span></span>|<span data-ttu-id="44dc1-138">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="44dc1-138">String</span></span>|<span data-ttu-id="44dc1-139">O título do aplicativo importado ou definido pelo administrador.</span><span class="sxs-lookup"><span data-stu-id="44dc1-139">The admin provided or imported title of the app.</span></span> <span data-ttu-id="44dc1-140">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="44dc1-140">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="44dc1-141">description</span><span class="sxs-lookup"><span data-stu-id="44dc1-141">description</span></span>|<span data-ttu-id="44dc1-142">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="44dc1-142">String</span></span>|<span data-ttu-id="44dc1-143">A descrição do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="44dc1-143">The description of the app.</span></span> <span data-ttu-id="44dc1-144">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="44dc1-144">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="44dc1-145">publisher</span><span class="sxs-lookup"><span data-stu-id="44dc1-145">publisher</span></span>|<span data-ttu-id="44dc1-146">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="44dc1-146">String</span></span>|<span data-ttu-id="44dc1-147">O publicador do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="44dc1-147">The publisher of the app.</span></span> <span data-ttu-id="44dc1-148">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="44dc1-148">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="44dc1-149">largeIcon</span><span class="sxs-lookup"><span data-stu-id="44dc1-149">largeIcon</span></span>|[<span data-ttu-id="44dc1-150">mimeContent</span><span class="sxs-lookup"><span data-stu-id="44dc1-150">mimeContent</span></span>](../resources/intune-shared-mimecontent.md)|<span data-ttu-id="44dc1-151">O ícone grande, a ser exibido nos detalhes do aplicativo e usado para o carregamento do ícone.</span><span class="sxs-lookup"><span data-stu-id="44dc1-151">The large icon, to be displayed in the app details and used for upload of the icon.</span></span> <span data-ttu-id="44dc1-152">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="44dc1-152">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="44dc1-153">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="44dc1-153">createdDateTime</span></span>|<span data-ttu-id="44dc1-154">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="44dc1-154">DateTimeOffset</span></span>|<span data-ttu-id="44dc1-155">A data e a hora da criação do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="44dc1-155">The date and time the app was created.</span></span> <span data-ttu-id="44dc1-156">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="44dc1-156">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="44dc1-157">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="44dc1-157">lastModifiedDateTime</span></span>|<span data-ttu-id="44dc1-158">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="44dc1-158">DateTimeOffset</span></span>|<span data-ttu-id="44dc1-159">A data e a hora que o aplicativo foi modificado pela última vez.</span><span class="sxs-lookup"><span data-stu-id="44dc1-159">The date and time the app was last modified.</span></span> <span data-ttu-id="44dc1-160">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="44dc1-160">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="44dc1-161">isFeatured</span><span class="sxs-lookup"><span data-stu-id="44dc1-161">isFeatured</span></span>|<span data-ttu-id="44dc1-162">Booliano</span><span class="sxs-lookup"><span data-stu-id="44dc1-162">Boolean</span></span>|<span data-ttu-id="44dc1-163">O valor que indica se o aplicativo está marcado como em destaque pelo administrador. Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="44dc1-163">The value indicating whether the app is marked as featured by the admin. Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="44dc1-164">privacyInformationUrl</span><span class="sxs-lookup"><span data-stu-id="44dc1-164">privacyInformationUrl</span></span>|<span data-ttu-id="44dc1-165">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="44dc1-165">String</span></span>|<span data-ttu-id="44dc1-166">A URL da declaração de privacidade.</span><span class="sxs-lookup"><span data-stu-id="44dc1-166">The privacy statement Url.</span></span> <span data-ttu-id="44dc1-167">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="44dc1-167">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="44dc1-168">informationUrl</span><span class="sxs-lookup"><span data-stu-id="44dc1-168">informationUrl</span></span>|<span data-ttu-id="44dc1-169">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="44dc1-169">String</span></span>|<span data-ttu-id="44dc1-170">A URL de informações adicionais.</span><span class="sxs-lookup"><span data-stu-id="44dc1-170">The more information Url.</span></span> <span data-ttu-id="44dc1-171">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="44dc1-171">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="44dc1-172">owner</span><span class="sxs-lookup"><span data-stu-id="44dc1-172">owner</span></span>|<span data-ttu-id="44dc1-173">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="44dc1-173">String</span></span>|<span data-ttu-id="44dc1-174">O proprietário do conteúdo.</span><span class="sxs-lookup"><span data-stu-id="44dc1-174">The owner of the app.</span></span> <span data-ttu-id="44dc1-175">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="44dc1-175">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="44dc1-176">developer</span><span class="sxs-lookup"><span data-stu-id="44dc1-176">developer</span></span>|<span data-ttu-id="44dc1-177">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="44dc1-177">String</span></span>|<span data-ttu-id="44dc1-178">O desenvolvedor do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="44dc1-178">The developer of the app.</span></span> <span data-ttu-id="44dc1-179">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="44dc1-179">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="44dc1-180">Observações</span><span class="sxs-lookup"><span data-stu-id="44dc1-180">notes</span></span>|<span data-ttu-id="44dc1-181">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="44dc1-181">String</span></span>|<span data-ttu-id="44dc1-182">Anotações para o aplicativo.</span><span class="sxs-lookup"><span data-stu-id="44dc1-182">Notes for the app.</span></span> <span data-ttu-id="44dc1-183">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="44dc1-183">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="44dc1-184">uploadState</span><span class="sxs-lookup"><span data-stu-id="44dc1-184">uploadState</span></span>|<span data-ttu-id="44dc1-185">Int32</span><span class="sxs-lookup"><span data-stu-id="44dc1-185">Int32</span></span>|<span data-ttu-id="44dc1-186">O estado de carregamento.</span><span class="sxs-lookup"><span data-stu-id="44dc1-186">The upload state.</span></span> <span data-ttu-id="44dc1-187">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="44dc1-187">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="44dc1-188">publishingState</span><span class="sxs-lookup"><span data-stu-id="44dc1-188">publishingState</span></span>|[<span data-ttu-id="44dc1-189">mobileAppPublishingState</span><span class="sxs-lookup"><span data-stu-id="44dc1-189">mobileAppPublishingState</span></span>](../resources/intune-apps-mobileapppublishingstate.md)|<span data-ttu-id="44dc1-190">O estado de publicação para o aplicativo.</span><span class="sxs-lookup"><span data-stu-id="44dc1-190">The publishing state for the app.</span></span> <span data-ttu-id="44dc1-191">O aplicativo não pode ser assinado, a menos que ele seja publicado.</span><span class="sxs-lookup"><span data-stu-id="44dc1-191">The app cannot be assigned unless the app is published.</span></span> <span data-ttu-id="44dc1-192">Herdada do [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="44dc1-192">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md).</span></span> <span data-ttu-id="44dc1-193">Os valores possíveis são: `notPublished`, `processing`, `published`.</span><span class="sxs-lookup"><span data-stu-id="44dc1-193">Possible values are: `notPublished`, `processing`, `published`.</span></span>|
|<span data-ttu-id="44dc1-194">packageId</span><span class="sxs-lookup"><span data-stu-id="44dc1-194">packageId</span></span>|<span data-ttu-id="44dc1-195">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="44dc1-195">String</span></span>|<span data-ttu-id="44dc1-196">O identificador do pacote.</span><span class="sxs-lookup"><span data-stu-id="44dc1-196">The package identifier.</span></span>|
|<span data-ttu-id="44dc1-197">appIdentifier</span><span class="sxs-lookup"><span data-stu-id="44dc1-197">appIdentifier</span></span>|<span data-ttu-id="44dc1-198">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="44dc1-198">String</span></span>|<span data-ttu-id="44dc1-199">O Nome da Identidade.</span><span class="sxs-lookup"><span data-stu-id="44dc1-199">The Identity Name.</span></span>|
|<span data-ttu-id="44dc1-200">usedLicenseCount</span><span class="sxs-lookup"><span data-stu-id="44dc1-200">usedLicenseCount</span></span>|<span data-ttu-id="44dc1-201">Int32</span><span class="sxs-lookup"><span data-stu-id="44dc1-201">Int32</span></span>|<span data-ttu-id="44dc1-202">O número de aplicativos VPP em uso.</span><span class="sxs-lookup"><span data-stu-id="44dc1-202">The number of VPP licenses in use.</span></span>|
|<span data-ttu-id="44dc1-203">totalLicenseCount</span><span class="sxs-lookup"><span data-stu-id="44dc1-203">totalLicenseCount</span></span>|<span data-ttu-id="44dc1-204">Int32</span><span class="sxs-lookup"><span data-stu-id="44dc1-204">Int32</span></span>|<span data-ttu-id="44dc1-205">O número total de licenças VPP.</span><span class="sxs-lookup"><span data-stu-id="44dc1-205">The total number of VPP licenses.</span></span>|
|<span data-ttu-id="44dc1-206">appStoreUrl</span><span class="sxs-lookup"><span data-stu-id="44dc1-206">appStoreUrl</span></span>|<span data-ttu-id="44dc1-207">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="44dc1-207">String</span></span>|<span data-ttu-id="44dc1-208">Tocar para a URL do aplicativo de repositório de trabalho.</span><span class="sxs-lookup"><span data-stu-id="44dc1-208">The Play for Work Store app URL.</span></span>|



## <a name="response"></a><span data-ttu-id="44dc1-209">Resposta</span><span class="sxs-lookup"><span data-stu-id="44dc1-209">Response</span></span>
<span data-ttu-id="44dc1-210">Se tiver êxito, este método retornará um `200 OK` código de resposta e um objeto atualizado [androidForWorkApp](../resources/intune-apps-androidforworkapp.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="44dc1-210">If successful, this method returns a `200 OK` response code and an updated [androidForWorkApp](../resources/intune-apps-androidforworkapp.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="44dc1-211">Exemplo</span><span class="sxs-lookup"><span data-stu-id="44dc1-211">Example</span></span>
### <a name="request"></a><span data-ttu-id="44dc1-212">Solicitação</span><span class="sxs-lookup"><span data-stu-id="44dc1-212">Request</span></span>
<span data-ttu-id="44dc1-213">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="44dc1-213">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceAppManagement/mobileApps/{mobileAppId}
Content-type: application/json
Content-length: 799

{
  "displayName": "Display Name value",
  "description": "Description value",
  "publisher": "Publisher value",
  "largeIcon": {
    "@odata.type": "microsoft.graph.mimeContent",
    "type": "Type value",
    "value": "dmFsdWU="
  },
  "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
  "isFeatured": true,
  "privacyInformationUrl": "https://example.com/privacyInformationUrl/",
  "informationUrl": "https://example.com/informationUrl/",
  "owner": "Owner value",
  "developer": "Developer value",
  "notes": "Notes value",
  "uploadState": 11,
  "publishingState": "processing",
  "packageId": "Package Id value",
  "appIdentifier": "App Identifier value",
  "usedLicenseCount": 0,
  "totalLicenseCount": 1,
  "appStoreUrl": "https://example.com/appStoreUrl/"
}
```

### <a name="response"></a><span data-ttu-id="44dc1-214">Resposta</span><span class="sxs-lookup"><span data-stu-id="44dc1-214">Response</span></span>
<span data-ttu-id="44dc1-p117">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="44dc1-p117">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 963

{
  "@odata.type": "#microsoft.graph.androidForWorkApp",
  "id": "c5010785-0785-c501-8507-01c5850701c5",
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
  "packageId": "Package Id value",
  "appIdentifier": "App Identifier value",
  "usedLicenseCount": 0,
  "totalLicenseCount": 1,
  "appStoreUrl": "https://example.com/appStoreUrl/"
}
```





