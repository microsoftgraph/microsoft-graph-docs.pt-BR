---
title: Tipo de número remoteAssistanceOnboardingStatus
description: O status atual do conector teamViewer
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: enumPageType
ms.openlocfilehash: 9ddd6d2884ef44a70f424de6d7e23d6bd6a3e94d
ms.sourcegitcommit: cd8611227a84db21449ab0ad40bedb665dacb9bb
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 10/18/2021
ms.locfileid: "60448945"
---
# <a name="remoteassistanceonboardingstatus-enum-type"></a>Tipo de número remoteAssistanceOnboardingStatus

Namespace: microsoft.graph

> **Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.

O status atual do conector teamViewer

## <a name="members"></a>Membros
|Membro|Valor|Descrição|
|:---|:---|:---|
|notOnboarded|0|O status relatado quando não há um conector TeamViewer ativo configurado ou ativo|
|integração|1|O status relatado quando o sistema iniciou uma conexão TeamViewer, mas o serviço ainda não concluiu a confirmação de um conector|
|onboarded|2|O status relatado quando o sistema troca com êxito informações de conta com o TeamViewer e agora pode iniciar sessões de assistência remota com clientes|



