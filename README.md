# simple-memo

실행: https://kanbada38-dotcom.github.io/simple-memo/ 접속 → 이메일·비밀번호 회원가입 또는 로그인 → 메모 입력·저장·삭제.

2026-10-30 실제 배포 사이트 검증: 첫 화면, 회원가입·자동 로그인, 저장·목록, 새로고침 후 로그인·메모 유지, 삭제, 로그아웃·재로그인 모두 통과.
RLS 활성화 및 본인 SELECT/INSERT/DELETE 정책 확인. authenticated 역할로 타 사용자 조회·삭제 차단과 소유자 위조 INSERT 거부 확인(검증 트랜잭션 rollback).
HTML 태그는 일반 텍스트로 표시. 공개 publishable 키만 사용.

기존 빈 실습 프로젝트 lcnelusmqhcdklxajcsv 재사용(설정 전 Auth 사용자 0명·public 테이블 없음). SAJU는 변경하지 않음. 실습용으로 이메일 확인 해제.
기능 미해결 사항 없음. 기존 Auth 경고: 유출 비밀번호 차단 비활성화([안내](https://supabase.com/docs/guides/auth/password-security#password-strength-and-leaked-password-protection)).
