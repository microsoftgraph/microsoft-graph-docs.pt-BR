---
title: Tipo de recurso dataSharingConsent
description: Informações de consentimento de compartilhamento de dados.
author: dougeby
ms.localizationpriority: medium
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 92c012f994c3e5aa3630f05632d48df764a432d7
ms.sourcegitcommit: 6c04234af08efce558e9bf926062b4686a84f1b2
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/12/2021
ms.locfileid: "59057324"
---
# <a name="datasharingconsent-resource-type"></a>Tipo de recurso dataSharingConsent

Namespace: microsoft.graph

> **Importante:** As APIs Graph Microsoft na versão /beta estão sujeitas a alterações; não há suporte para uso de produção.

> **Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.

Informações de consentimento de compartilhamento de dados.

## <a name="methods"></a>Métodos
|Método|Tipo de retorno|Descrição|
|:---|:---|:---|
|[Listar dadosSharingConsents](../api/intune-devices-datasharingconsent-list.md)|[Coleção dataSharingConsent](../resources/intune-devices-datasharingconsent.md)|Listar propriedades e relações dos [objetos dataSharingConsent.](../resources/intune-devices-datasharingconsent.md)|
|[Obter dadosSharingConsent](../api/intune-devices-datasharingconsent-get.md)|[dataSharingConsent](../resources/intune-devices-datasharingconsent.md)|Ler propriedades e relações do [objeto dataSharingConsent.](../resources/intune-devices-datasharingconsent.md)|
|[Criar dataSharingConsent](../api/intune-devices-datasharingconsent-create.md)|[dataSharingConsent](../resources/intune-devices-datasharingconsent.md)|Crie um novo [objeto dataSharingConsent.](../resources/intune-devices-datasharingconsent.md)|
|[Excluir dataSharingConsent](../api/intune-devices-datasharingconsent-delete.md)|Nenhum|Exclui um [dataSharingConsent](../resources/intune-devices-datasharingconsent.md).|
|[Atualizar dataSharingConsent](../api/intune-devices-datasharingconsent-update.md)|[dataSharingConsent](../resources/intune-devices-datasharingconsent.md)|Atualize as propriedades de [um objeto dataSharingConsent.](../resources/intune-devices-datasharingconsent.md)|
|[Ação consentToDataSharing](../api/intune-devices-datasharingconsent-consenttodatasharing.md)|[dataSharingConsent](../resources/intune-devices-datasharingconsent.md)|Ainda não documentado|

## <a name="properties"></a>Propriedades
|Propriedade|Tipo|Descrição|
|:---|:---|:---|
|id|Cadeia de caracteres|A ID de consentimento de compartilhamento de dados|
|serviceDisplayName|Cadeia de Caracteres|O nome de exibição do fluxo de trabalho do serviço|
|termsUrl|Cadeia de Caracteres|The TermsUrl for the data sharing consent|
|concedido|Boleano|O estado concedido para o consentimento de compartilhamento de dados|
|grantDateTime|DateTimeOffset|O consentimento de hora foi concedido para essa conta|
|grantedByUpn|Cadeia de Caracteres|O Upn do usuário que concedeu consentimento para essa conta|
|grantedByUserId|Cadeia de Caracteres|UserId do usuário que concedeu consentimento para essa conta|

## <a name="relationships"></a>Relações
Nenhum

## <a name="json-representation"></a>Representação JSON
Veja a seguir uma representação JSON do recurso.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.dataSharingConsent"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.dataSharingConsent",
  "id": "String (identifier)",
  "serviceDisplayName": "String",
  "termsUrl": "String",
  "granted": true,
  "grantDateTime": "String (timestamp)",
  "grantedByUpn": "String",
  "grantedByUserId": "String"
}
```



